# How to contribute to this tutorial repository

Thank you for considering contributing to this tutorial repository!

## Support questions

[](CONTRIBUTE.md#support-questions)

Please don't use the issue tracker for this. The issue tracker is a tool to address bugs and feature requests for the project itself. 

Use one of the following resources for questions about the project:

- Ask on our [GitHub Discussions](https://github.com/AdyGCode/Intro-to-Version-Control/discussions/) for long term discussion or larger questions.

## Reporting issues

[](https://github.com/pallets/flask/blob/main/CONTRIBUTING.rst#reporting-issues)

Include the following information in your post:

- Before reporting a problem, check if this issue is already fixed in the latest releases or the latest code in the repository.
- Provide a title that gives a basic indicator of the yuou have. For example "Content missing: Chapter 7 No content", or "Grammar: Chapter 4"
- Provide a possible solution, if you are able to do so. 

## Submitting patches

[](https://github.com/pallets/flask/blob/main/CONTRIBUTING.rst#submitting-patches)

If there is not an open issue for what you want to submit, prefer opening one for discussion before working on a PR. You can work on any issue that doesn't have an open PR linked to it or a maintainer assigned to it. These show up in the sidebar. No need to ask if you can work on an issue that interests you.

Include the following in your patch:

- Update any relevant documents and images.
- Add an entry in `CHANGELOG.md`. Use the same style as other entries.

### First time setup in your local environment

[](https://github.com/pallets/flask/blob/main/CONTRIBUTING.rst#first-time-setup-in-your-local-environment)

- Make sure you have a [GitHub account](https://github.com/join).

- Download and install the [latest version of git](https://git-scm.com/downloads).

- Configure git with your [username](https://docs.github.com/en/github/using-git/setting-your-username-in-git) and [email](https://docs.github.com/en/github/setting-up-and-managing-your-github-user-account/setting-your-commit-email-address).
    ```bash
git config --global user.name 'your name'
git config --global user.email 'your email'
```

- Fork this repository to your GitHub account by clicking the [Fork](https://github.com/AdyGCode/Intro-to-Version-Control/fork) button.

- [Clone](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo#step-2-create-a-local-clone-of-your-fork) your fork locally, replacing `your-username` in the command below with your actual username.
```bash
git clone https://github.com/your-username/Intro-to-Version-Control.git
cd Intro-to-Version-Control
```


### Start Editing and Documenting

[](https://github.com/pallets/flask/blob/main/CONTRIBUTING.rst#start-coding)

- Create a branch to identify the issue you would like to work on using the following rules:

	- If you are adding a new chapter, branch off the `dev` branch. Name your branch `feat/feature_name`.

  
```bash
git fetch origin
git checkout -b feat/feature_name origin/2.0.x
```

  - If you're submitting a bug or documentation fix, branch off of the latest main branch. Name your fix `fix/`
  

    
    
    
    If you're submitting a feature addition or change, branch off of the "main" branch.
    
    $ git fetch origin
    $ git checkout -b your-branch-name origin/main
    
- Using your favorite editor, make your changes, [committing as you go](https://afraid-to-commit.readthedocs.io/en/latest/git/commandlinegit.html#commit-your-changes).
    
    - If you are in a codespace, you will be prompted to [create a fork](https://docs.github.com/en/codespaces/developing-in-codespaces/using-source-control-in-your-codespace#about-automatic-forking) the first time you make a commit. Enter `Y` to continue.
- Include tests that cover any code changes you make. Make sure the test fails without your patch. Run the tests as described below.
    
- Push your commits to your fork on GitHub and [create a pull request](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request). Link to the issue being addressed with `fixes #123` in the pull request description.
    
    $ git push --set-upstream origin your-branch-name
    

### Building the docs

[](https://github.com/pallets/flask/blob/main/CONTRIBUTING.rst#building-the-docs)

Build the docs in the `docs` directory using Sphinx.

$ cd docs
$ make html

Open `_build/html/index.html` in your browser to view the docs.

Read more about [Sphinx](https://www.sphinx-doc.org/en/stable/).