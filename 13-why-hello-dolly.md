# Hello, Dolly. The Clone

One of the processes that you will use is that of cloning.

Cloning makes a complete copy of a repository and saves it locally. This includes the history of changes that have been committed to the repo.

When cloning there is one BIG warning to be noted:

> **WARNING**: Do not clone into an existing repository's folder.
> 
> This can be achieved by always starting at the `Source/Repos` folder we use.

We are able to clone by:
- New Empty Folder, Clone into new folder
- New Empty Folder, Change into folder, Clone to this folder
- Clone directly into a new folder

> *For these examples we will clone the repository that contains these notes.*

## Clone Directly Into New Folder of Same Name

Make sure you are in the `Source/Repos` folder.

The general command is:

```shell
git clone https://github.com/PROFILE_NAME/REPOSITORY_NAME.git
```

This will clone the repository into a new folder called `REPOSITORY_NAME`.

Example: Clone the Intro-to-Version-Control repo:
```shell
git clone https://github.com/AdyGCode/Intro-to-Version-Control.git
```

## Clone Directly Into Different Folder

Make sure you are in the `Source/Repos` folder.

The general command is:

```shell
git clone https://github.com/PROFILE_NAME/REPOSITORY_NAME.git NEW_REPOSITORY_FOLDER_NAME
```

This will create a new folder called NEW_REPOSITORY_FOLDER_NAME and then clone the repository into it.

Example: Clone the Intro-to-Version-Control repo into a new folder called `my-intro-to-git`:
```shell
git clone https://github.com/AdyGCode/Intro-to-Version-Control.git my-intro-to-git
```

## Create a Folder and Make Clone

Make sure you are in the `Source/Repos` folder.

The general commands are:

```shell
mkdir NEW_REPOSITORY_FOLDER_NAME
git clone https://github.com/PROFILE_NAME/REPOSITORY_NAME.git NEW_REPOSITORY_FOLDER_NAME
```

This will clone the repository into the folder called `NEW_REPOSITORY_FOLDER_NAME`.

Example: Clone the Intro-to-Version-Control repo:
```shell
git clone https://github.com/AdyGCode/Intro-to-Version-Control.git
```

## Create a Folder, Switch Folders and Make Clone

Make sure you are in the `Source/Repos` folder.

The general commands are:

```shell
mkdir NEW_REPOSITORY_FOLDER_NAME
cd NEW_REPOSITORY_FOLDER_NAME
git clone https://github.com/PROFILE_NAME/REPOSITORY_NAME.git .
```

This will clone the repository into the folder called `NEW_REPOSITORY_FOLDER_NAME`.

Example: Clone the Intro-to-Version-Control repo:
```shell
mkdir my-intro-to-git
cd my-intro-to-git
git clone https://github.com/AdyGCode/Intro-to-Version-Control.git .
```


