# Shaking the Tree

Git allows us to try things out without affecting our working code. This ability is known as branching.

The main branch is sometimes called the 'trunk', and like any tree trunk, it has branches that split off from it.

Unlike trees, branches in version control may merge back into the trunk.

But this is not just for the trunk, a branch may have branches split off from it, and allow for testing on an idea
before it is added back into the branch if the idea solves that particular problem.

## Creating a branch

We usually create a branch when we want to work on an idea that is not certain to work, or if we need to test an idea.

When possible this is done after a commit, but it may be done at any time, if needed.

To create a branch we use:

```shell
git branch BRANCH_NAME
```

For example:

```shell
git branch feat-readme
```

## Switching Branches

Next we need to switch to the branch to work on it:

```shell
git switch BRANCH_NAME
```

For example:

```shell
git switch feat-readme
```

You are now able to work on the code in this new branch.

At any point you have code that is working, you may add to the staging area and commit the file or files.
