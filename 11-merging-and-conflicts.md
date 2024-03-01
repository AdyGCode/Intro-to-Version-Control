## Merging a Branch into "main"

To merge the branch you were working on into the main branch, we do the following steps:

```shell
git switch main

git merge BRANCH_NAME
```

For example:

```shell
git switch main
git merge feat-readme
```

## EEK! I've got Conflicts!

Not all merges will go smoothly, and you may end up with conflicts in your code.

This often happens when you have been working on the main branch and your development branch and have committed changes on both.

To resolve this we need to edit the file(s) with the errors and fix the changes by accepting the code that is correct, or most relevant to the project.

The image below shows the conflict being reported.

![[pasted-image-20240223114440.png]]

To resolve the conflicts you now edit the file (or files) with the conflicts.

Opening the file will reveal the conflicting code highlighted using `<<<<<<` and `>>>>>>` to show the 'direction' the changes come from (and the branch), and `======` to show where the changes end/start.

Here is an example:

```text

<<<<<<< HEAD

Text from the version in the HEAD (main) branch

=======

Text from the version in the feature-1 branch

>>>>>>> feature-1
```

Opening the required file and accepting lines of code (leaving them in) and rejecting lines of code (deleting them) helps resolve the conflict.

The final steps of this resolution are to remove the `>>>>>>`, `======` and the `>>>>>>` lines, save the changes and close the file.

At this point you are able to add and commit the now resolved conflict:

```shell
git add FILE_NAME
git commit -m "MERGE SUMMARY MESSAGE"
```

The image below shows a really bad commit message:

![[pasted-image-20240223115404.png]]

If we now log the commits we will see a diagram of the branches with the conflict shown in red:

![[pasted-image-20240223115456.png]]
