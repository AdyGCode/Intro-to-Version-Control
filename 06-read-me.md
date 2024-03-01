## Creating a `ReadMe.md` for the project

The Bash/git shell has the ability to create a empty file really easily. 

For example an empty `ReadMe.md` file would be created using:

```shell
touch ReadMe.md
```

In the Windows Command Prompt we need to use:

```shell
copy nul > ReadMe.md
```

The `>` tells the command to write to a file with the name of the file after the `>`.

If you used `>>` it would append the output of the command to the file named after the `>>`.
