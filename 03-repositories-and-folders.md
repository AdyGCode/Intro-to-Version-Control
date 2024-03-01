# Repositories and Folders

Projects are contained in a folder in your user's root/home folder.

This folder is the `Source/Repos` folder.

If you do not have this folder then the steps below should be followed.

## Creating a `Source/Repos` folder structure for projects

Open Terminal and then click the `v` next to the `+` on the tab bar.

Select the *Command Prompt* option

![[pasted-image-20240216105215.png]]

When the terminal opens use the following commands to change into your "user home" and make the `Source\Repos` folder.

> **Important:** We tend to use the forward slash `/` in notes as they show up easily, plus most operating systems other than Windows use the `/` as the folder separator. 
> 
> Later you will see this in action when using the Git command line.

Here are the commands to use:
```shell
cd %userprofile%
mkdir Source 
mkdir Source\Repos
```
You should now have the folders created.

Check this using:
```shell
dir Source\Repos
```
It should show a folder listing with no files.
