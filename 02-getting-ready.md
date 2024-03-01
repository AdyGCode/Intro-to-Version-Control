# Required Software

Before you start using Git you will need some software to be installed.

For Windows users the combination is one of:
- Microsoft Terminal and Git-SCM, or
- Microsoft Terminal and Laragon

For MacOS users then either:
- iTerm2 & Git, or
- Warp & Git

Mac users are able to install Git via the Git-SCM installer or via homebrew.

For Linux users:
- Git
Linux users should find git installed, if not use the package manager appropriate for your version of Linux.

## Windows Installations

### Microsoft Terminal Installation

This is a great way to interact with the command line.

Open the Microsoft Store, and search for "Microsoft Terminal".

Install the "Microsoft Terminal" version and not the preview.

### Git Installation

Easiest way is to download and use the Git SCM installer:

https://git-scm.com/download/win

Use the 64 Bit version when possible.

Run the installer and accept the defaults.

### Laragon Installation

Download the Full Installer from https://laragon.org/download/index.html.

Run the installer and accept the defaults.

This places Laragon in the folder `c:\Laragon`.

# The CLI

CLI stands for Command Line Interpreter.

There are many of them including:
- Windows Command Prompt
- Microsoft PowerShell
- bash 
- zshell
- and many more

## Parts of the Prompt

| Image                                              | Description |
|----------------------------------------------------| ---- |
| ![](./assets/pasted-image-20240216111739.png)     | This is the user account, followed by the computer name and separated by an `@`<br><br>Literally: *User **at** Computer*<br>  |
| ![](./assets/pasted-image-20240216111840.png)     | Tells us that we are running in MinGW 64 bit<br>  |
| ![](./assets/pasted-image-20240216111909.png) | Shows we are in the `~/Source/Repos` folder, where `~` is the user's (your) home folder.<br><br>In Windows terms, this is the same as:<br><br>  `C:\Users\UserName\Source\Repos`<br>  |

## Setting up Microsoft Terminal to use Git Bash as a CLI

Open MS Terminal.

Click on the `v`  (or press `CTRL`+`,`) on the tab bar.

Click *Settings*...

![](./assets/pasted-image-20240216103325.png)

Click on *Add a new profile*...

![](./assets/pasted-image-20240216103615.png)

Click *New Empty Profile*...

![](./assets/pasted-image-20240216103644.png)

Click on the `v` next to the "*Profile x*"...

![](./assets/pasted-image-20240216103947.png)

And give the profile a name...

![](./assets/pasted-image-20240216103833.png)

Next find the *Command Line* entry and click on the `v`

![](./assets/pasted-image-20240216104034.png)

Then click the *Browse* button...

![](./assets/pasted-image-20240216104105.png)

At home, if you have installed using Git-SCM installer then the default location for Git is: `c:\program files\git`. If you have Laragon installed using the default installation location, then you should find Git in the `C:\Laragon\bin\git` folder.

> At TAFE, we have a different location, `c:\ProgramData\git` or even `C:\ProgramData\Laragon\bin\git`.

Use the browse to locate the folder and find either the `git.exe` or the `bash.exe` file in the `bin` folder.

![](./assets/pasted-image-20240216105026.png)

Click on the Starting Directory `v` and then untick the "*Use parent process directory*"...

![](./assets/pasted-image-20240216105847.png) 
This should then show `%USERPROFILE%` in a text field and `Browse` button underneath... 

![](./assets/pasted-image-20240216105903.png)

No matter what is shown, clear the content and enter the following in its place...

`%USERPROFILE%\Source\Repos`

![](./assets/pasted-image-20240216110033.png)

Click `SAVE` to save the changes

### Visual flair (optional)
You may optionally customise the appearance of the terminal. 

Adrian tends to do this to visually identify the various prompts.

The steps below are optional, and you may vary to your own "taste".

Click the *Appearance* item.

![](./assets/pasted-image-20240216110837.png)

You may change the base colour scheme, the font face and more.

Here are the settings Adrian has for this terminal prompt:

![](./assets/pasted-image-20240216110957.png)

Click Save then you can click the `X` next to settings to close the dialog.
![](./assets/pasted-image-20240216111033.png)

Finally you are able to open the new terminal by clicking on the `v` and selecting your custom terminal or using the short-cut it shows on the right next to your custom terminal.

![](./assets/pasted-image-20240216111111.png)

You will now have your terminal open and ready:

![](./assets/pasted-image-20240216111239.png)


# Advanced Users

If you want to make your CLI look even cooler (more useful) then something like OhMyPosh (https://ohmyposh.dev/) may help.
