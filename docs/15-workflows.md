# Version Controlled Workflows

The video by Nick Chapsas "Getting started with branching workflows, Git Flow and GitHub Flow" provides a summary of these two workflows.

[Getting started with branching workflows, Git Flow and GitHub Flow (youtube.com)](https://www.youtube.com/watch?v=gW6dFpTMk8s)


## Git Flow Workflow

Git Flow is a branching model that helps teams manage their codebase more efficiently. 

It's like having a playbook for how to organize your work and collaborate with others on a project. 

Here's how it works:

1. **Main Branches**: There are two main branches:
    - `main` (or `master`): This is the branch that contains the production-ready code.
    - `develop`: This is the branch where all the new features and bug fixes are integrated before being merged into the `main` branch.
2. **Supporting Branches**: There are also supporting branches for specific tasks:
    - `feature` branches: These branches are used to develop new features. When a feature is complete, it is merged back into the `develop` branch.
    - `release` branches: When the `develop` branch is stable and ready for a release, a `release` branch is created from it. This is where any last-minute bug fixes or documentation updates are made before the release is merged into the `main` branch and tagged with a version number.
    - `hotfix` branches: These branches are used to quickly fix critical issues in the production code (`master` branch). When the fix is complete, it is merged back into both the `main` and `develop` branches.

This workflow helps keep the `main` branch stable, while allowing active development to happen in parallel on the `develop` branch and other supporting branches.


## GitHub Flow Workflow

GitHub Flow is a simpler branching model compared to Git Flow. 

It's designed to work well with GitHub's features and allows for more frequent deployments. 

Here's how it works:

1. **Main Branch**: There is only one main branch, typically called `main` or `master`.
2. **Feature Branches**: Whenever you want to work on a new feature or bug fix, you create a new branch from the `main` branch.
3. **Pull Requests**: When you're ready to merge your changes back into the `main` branch, you create a Pull Request. This allows others to review your code and provide feedback before merging.
4. **Code Reviews**: The Pull Request triggers a code review process, where team members can discuss the changes, suggest improvements, or request additional changes.
5. **Merge and Deploy**: Once the code has been reviewed and approved, the feature branch is merged into the `main` branch. This merged code can then be deployed to production.

GitHub Flow encourages frequent, small updates to the codebase, making it easier to manage and integrate changes.

## Further Reading and Tutorials

Select one or two to review and make notes about.

Feel free to feedback as to what you think about the selected items.

- [Guide to Git Flow (gitdailies.com)](https://gitdailies.com/articles/git-flow-guide/)
- [Git Workflow | Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials/comparing-workflows)
- [How To Use Git Flow Effectively (marketsplash.com)](https://marketsplash.com/tutorials/git/git-flow/)
- [Git Flow | Developer Experience Knowledge Base](https://developerexperience.io/articles/git-flow)
- [Getting started with Git using SourceTree - YouTube](https://www.youtube.com/playlist?list=PLpL2ONl1hMLtlY1Y7YJNcA5zumvaITLYs)
- [The Gitflow Release Branch from Start to Finish (youtube.com)](https://www.youtube.com/watch?v=rX80eKPdA28)
- [What is Git Flow | How to use Git Flow | Learn Git (gitkraken.com)](https://www.gitkraken.com/learn/git/git-flow)
- [git-flow cheatsheet (danielkummer.github.io)](https://danielkummer.github.io/git-flow-cheatsheet/)
- [A successful Git branching model » nvie.com](https://nvie.com/posts/a-successful-git-branching-model/)
- [GitHub Flow: A Quick 5-Step Process (hubspot.com)](https://blog.hubspot.com/website/github-flow)
- [Intro to GitHub Flow - GitHub Education](https://education.github.com/experiences/series_intro_github_flow)
- [Understanding GitHub Flow: A Comprehensive Guide (gyata.ai)](https://www.gyata.ai/github/github-flow/)
- [Understanding the GitHub Flow | GitHub Guides (gitbooks.io)](https://roachhd.gitbooks.io/github-guides/content/flow/flow.html)
- [Git Flow vs GitHub Flow | Alex Hyett](https://www.alexhyett.com/git-flow-github-flow/)
- [Git Flow vs GitHub Flow: What You Need to Know (youtube.com)](https://www.youtube.com/watch?v=hG_P6IRAjNQ&feature=youtu.be)
- 
- 