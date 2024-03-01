## Checking the Status of the Repo

Checking the status of the repository is done using the `git status` command:

```shell
git status
```
![[pasted-image-20240216121457.png]]

In this example, we have two files that are not "tracked" by the repository.

Untracked files are shown in Red, tracked in green.

## Adding a file for tracking

To add a file to be tracked we use `git add FILENAME`. For example:

```shell
git add ReadMe.md
```
![[pasted-image-20240216121921.png]]

Checking the status after adding shows:

![[pasted-image-20240216122006.png]]

Once a file is tracked, any time you make changes and are happy with them, you should perform a `git status` and then `git add` the changed file.

![[pasted-image-20240216122531.png]]

Here you see the file has been modified.

![[pasted-image-20240216122620.png]]

After adding the changes, we see it is back to  'new'.

## Committing a file to history

Committing files to the repo, makes them available as a chapter in the project's history.

To commit changes we use:

```shell
git commit -m "Commit message"
```

In the above line the `-m` indicates that we are including a message.

![[pasted-image-20240216122842.png]]

Now our `git status` should show:

![[pasted-image-20240216123105.png]]

The committed file is still tracked, but as no changes have been made it does not show. 

> **Best Practice Hint:** Note in my message, that I included `init:` at the start. This is telling me (and anyone who is on the project) that it is the initialisation of the project. 
> 
> If it is a new feature we use `feat` instead and often would add the feature name in `( )` round brackets. More on this later.

### Exercise

Run through the steps above.

Once complete, edit the `ReadMe.md` and add:

```markdown
## Summary
- Author: Adrian Gould
- Version: 1.0
```

Save the changes, then check the status of the repository.

It should show the `ReadMe.md` has changed:

![[pasted-image-20240216123506.png]]

**Add** the changes to the repo and **commit** them using the message:

```text
feat(readme): Update ReadMe.md to include author and version
```

![[pasted-image-20240216123759.png]]






### Did you forget `-m` on `git commit`?

If you type in `git commit` and do not add the `-m` with the message then the `vi` editor is shown.

The easiest way out is to do the following:

- **Option 1:** Press **`ESCAPE`** then type **`:qa`** - This is a quit and abandon changes. This is the better option.
  
- **Option 2:** Press **`ESCAPE`**, then press and hold the **`SHIFT`** whilst typing **`Z`** twice - This is a save and quit

![[pasted-image-20240216125345.png]]
