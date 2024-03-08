# Remotely Useful

So we have the basics of using Git, but at the moment all our versioned code is stuck on the local machine. That's not
very safe.

A way that we can get around this is to use a Version Control Repository that is hosted in the cloud, or as it is known
by most, a Remote.

A Remote is a copy of Git running on a server somewhere else, usually with a GUI front end, most commonly a Web-based
interface.

There are many repository management systems run both for free and profit. It is also possible to create a self hosted
web based repository management system.

Common (and less common) systems include:

- GitHub
- GitLab
- BitBucket
- Gitea
- GNU Savannah
- GitBucket
- Gogs

# GitHub

## Creating a GitHub account

Go to https://github.com/join and on the sign-up page enter your details.

When doing this, there are a couple of items to note:

- The username needs to be unique.
- You cannot reuse an email address.
- You may use a personal email address or your TAFE student email.
- Do NOT make the username offensive, as many prospective employers will look at your accounts!

![](assets/pasted-image-20240301120950.png)

The next step requires you to verify that you are not a bot by solving a puzzle.

Once the puzzle is solved, you will then need to verify your email address.

To do this GitHub will send you and email that contains a link. Opening this link will verify your email address.

![](assets/pasted-image-20240301121055.png)

Once you have verified your email address, you are all done and are now able to create your very first project on
GitHub.

![](assets/pasted-image-20240301121111.png)

## GitHub Repositories

If you have code already started for a project, then the best bet is to create an empty repository on GitHub.

In the majority of cases at TAFE you will have started on a project using your IDE to create the shell of the
application without any extra code. At this point you will then want to initialise the repository and push the initial
code to the remote.

> **Note:** If you try to do this with a remote repository that has files in it already, you will run into issues that
> require steps to "merge" the the remote and local together.
>
> This process is not as simple as the merge conflict resolution from chapter 11 (Merging and Conflicts).

### Creating an Empty GitHub Repo

To create an empty GitHub repository, we use the following steps:

Click on the "add new repository" button.
![[assets/2024-03-01_14_56_22-AdyGCode_git-remote-demo-Brave.png]]

Click New Repository
![[assets/2024-03-01_14_56_32-AdyGCode_git-remote-demo-Brave.png]]

Do **NOT** select a template...

![[assets/2024-03-01_14_57_21-New-repository-Brave.png]]

Give the Repository a meaningful name, making sure to use only letters, numbers and the minus sign.

![[assets/2024-03-01_14_57_02-New-repository-Brave.png]]

It is a good idea to give a short, one line description of the the repository.
![[assets/2024-03-01_14_57_15-New-repository-Brave.png]]

For general work, PUBLIC repositories are ok. For example for classwork that is not assessed, the Public Repo is the
choice to make.
![[assets/2024-03-01_14_57_29-New-repository-Brave.png]]

If you are working on an assessment make sure your repository is PRIVATE.
![[assets/2024-03-01_14_57_37-New-repository-Brave.png]]

Do not select any of the options for Add ReadMe, add .gitignore and do not choose a licence.
![[assets/2024-03-01_14_57_43-New-repository-Brave.png]]

Click on "Create Repository."
![[assets/2024-03-01_14_57_49-New-repository-Brave.png]]

Once you do this, then a new blank Repo is created:

![[assets/2024-03-01_15_03_52-AdyGCode_git-remote-demo-ii-Brave.png]]

Here is a short video showing the steps.

![](assets/brave_dWSQwZYc3F.mp4)

### Take Note of The "Quick Setup" Section

Once the repository is created it is a good idea to note down the details for the remote settings. (We presume you are
working on the main branch.)

```shell
git remote add origin https://github.com/AdyGCode/git-remote-demo-ii.git
git push -u origin main
```

# Remotes

A remote is a copy of a repository that exists elsewhere, be that on the same machine, the same network, or the Internet
via a web-based Version Control management application such as GitHub.

A remote that is seen as the "source of truth" for the project is usually known as the "origin".

When you have set up a repository on a system such as GitHub (from here on we presume GitHub), you attach your local
repository to the remote and use commands to fetch, merge, and push code to and from the remote.

## Attaching your Local Repo to the Remote

Once you have your local and remote ready, we can "attach" them.

The command to attach the local to remote is:

```shell
git remote add origin https://github.com/PROFILE_NAME/REPOSITORY_NAME.git
```

So for the demonstration above we use:

```shell
git remote add origin https://github.com/AdyGCode/git-remote-demo-ii.git
```

Once it is attached we then use the `git push` command to push the current commited code to the remote:

```shell
git push -u origin main
```

The `-u` indicates that the origin is the upstream location for main.

From this point, if you are working on a project and wish to push the main branch to the remote you can simply use:

```shell
git push
```
