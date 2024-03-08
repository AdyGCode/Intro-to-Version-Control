# Git Started

We are now ready to get started, and create a repository and work with it.

## Initialising a Repository for a 'project'

There are three main ways to start a project. 

Two of them presume you have no existing files to begin with, and the third when you have files in an existing folder.

- Create a folder (for the project) and initialise
- Initialise with folder (project) name
- Initialise with the existing folder and files

### Option 1: Create a folder then initialising

Use `mkdir` command to create the folder, change into the new folder, and then using the `git init .` command.

Let's presume the new project will be in the `Duck-Rogers` folder.

Use the `pwd` command to verify the folder:

![](pasted-image-20240216113101.png)

You see that the Windows `\` have been reversed to `/` and the `:` removed.

```shell
mkdir Duck-Rogers
cd Duck-Rogers
git init .
```

![](pasted-image-20240216113320.png)

The command prompt will now show either `(master)` or `(main)` - if it is `master`, we will show you later how to (a) change it to `main` for the current project and (b) to make `main` the default.

### Option 2: Initialise project and folder at same time

To create the `Duck-Rogers` folder and initialise in a single move, we do the following:

```shell
git init Duck-Rogers
cd Duck-Rogers
```

![](pasted-image-20240216113649.png)

![](pasted-image-20240216113804.png)

### Option 3: Initialise project with existing files

The best part of this is that you are basically able to use the previous options, except the folder already exists.

For example, if `Duck-Rogers` already exist and has files, then, if we are at the parent folder for  Duck-Rogers we can use the `git init Duck-Rogers` command.

![](pasted-image-20240216114404.png)

If you are in the `Duck-Rogers` folder and there are files in the folder then using the `git init .` command will do the same thing.

![](pasted-image-20240216114456.png)


## Verify Repository was Created

To check it is created we use the `ls -la` command:

![](pasted-image-20240216113831.png)

Notice the last line. The `d` at the start tells you it is a folder (directory), and its name is `.git`. It is a hidden folder.

All tracking of changes are then stored in the `.git` folder. If you delete this folder, you delete the whole history of your project.
