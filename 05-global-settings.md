## Global configuration changes

Git, like any software has many things that can be changed. These area stored in a global configuration file, in a project only configuration file.

Most of the configuration options are able to be set for both, but we show the global (for you as the user) changes you may want to make.

### Git User Name and Email Address

To change the username and email address being stored as part of the commit sequence, we use the following two commands:

```bash
git config --global user.name "YOUR NAME"
git config --global user.email "YOUR EMAIL ADDRESS"
```

The `--global` indicates that the changes are stored for this and all future projects.

![[pasted-image-20240216124422.png)

To see the global settings...
```shell
git config --list --global
```

![[pasted-image-20240216124543.png)

### Per Project Configuration

These need to be repeated for any project that is not going to be listed under your 'global' config.

Make sure you are in the project you wish to use project only configured settings.

Then set your required configuration by using:

```shell
git config SETTING VALUE
```

For example, changing the "user" and "email" to be your TAFE details rather than using your personal email and name...

Lets say your ID is `00000000` and email is `00000000@tafe.wa.edu.au` we could use:

```bash
git config user.name "00000000"
git config user.email "00000000@tafe.wa.edu.au"
```

The `--global` indicates that the changes are stored for this and all future projects.

![[pasted-image-20240216124422.png)


### Default "Branch" name to Main...

To do this for ALL FUTURE projects we use:

```bash
git config --global init.defaultBranch main
```
### Change Current Project's Branch Name

To change the current 'master branch' to be the 'main branch' we need to do the following *AFTER* a commit is completed:
```bash
git branch -m master main
```

![[pasted-image-20240216125018.png)






### Default Commit Message Editor

It is possible to change the code editor for commit messages to something like Notepad.

Below we change the editor to "nano" - a extremely small footprint terminal text editor on MacOS and Linux.

```shell
git config --global core.editor "nano"
```

To change it to Notepad we would use:

```shell
git config --global core.editor "notepad"
```

> **Important:** when using a GUI editor such as Notepad, you **MUST** **SAVE** and **CLOSE** the message, then (usually optionally) **QUIT** the application for the message to be transferred to the git command.

Now when you enter `git commit` the Notepad editor will open. The command line will tell you it is waiting for the editor to close a file (`COMMIT_MESSAGE`).

![[pasted-image-20240223102507.png)

When Notepad is opened, it will show a set of comments that tell you details about the added files as comments.

![[pasted-image-20240223102034.png)

Now editing the commit message and adding the details that may be more than just a one liner is easy.

You then enter the SHORT commit message and, as required, a blank line followed by more details about the changes that have been made to the project.

For example:

```text
feat(readme): Add demo commit demo of external editor

- Change config for default commit editor to Notepad
- Add a single blank line to the ReadMe for demo purposes
- Add ReadMe to staging
- Run git commit
- Demonstrate the long form of commit message
- Save (`CTRL`+`S`) and close (`CTRL`+`F4`) the message
- Optionally, quit the editor (`ALT`+`F4`)
```



> **Warning:** Tests have indicated that you will not be able to use 'VSCode' as the editor for messages. 
> 
> On execution the editor does not negotiate correctly with the command line and git aborts the commit.
