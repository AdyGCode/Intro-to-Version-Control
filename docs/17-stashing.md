# Stashing Changes

We all know what squirrels and other animals do, the put away food for harsh times. They create a secret stash.

Mush like this, Git also has the ability to stash.

Stashing is simply putting work aside whilst you do something else.

## Stashing

A common situation for the use of stashing is when uncommitted changes get in the way of branching.

This often occurs when one branch is ahead of your working copy. The act of switching to the other branch would then lead to git clobbering your changes.

Thankfully, Git will not let that happen.

So what do you do? Have a think how you could resolve the problem.

### This is one possible solution

So when the above scenario occurs you would have to:

- Copy the changes – you are not sure what files changed, so you probably grab everything (yuck!)
- Copy to another folder (yuck yuck)
- Use git reset --hard to DESTROY the working copy changes (yuck yuck yuck)
- Switch to the branch
- Do work
- Switch back, copy all the files back and really really hope you didn’t stuff everything up

### Or... Making Life Easier

That is both nasty and long winded... so we can make it easier by using a stash of changes:

- git stash
- switch
- switch back
- git stash pop

And there you have it... we are done!

## This is a Public Service Announcement

Git stash is sometimes not taught in an introduction to Git.

The problem with this it that it is just about the most useful command you can find to make working with Git seamless.

This is particularly true if you are branch/working with a remote, that is, using git as intended!

# Time for your Supplements

This video is on Git Stash... The audio at the start may be a little off centre.

<iframe width="560" height="315" src="https://www.youtube.com/embed/adzewZEj2Pg?si=KJKuu2p7pTi3soDL" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

# References

Adhikary, T. (2023). _10 Git stash commands every developer should know_. [online] GreenRoots Blog - Tapas Adhikary. Available at: https://blog.greenroots.info/10-git-stash-commands-every-developer-should-know [Accessed 15 Mar. 2024].

Programming Peanut (n.d.). _[Git] What is Git Stash and how to use it_. [online] www.youtube.com. Available at: https://www.youtube.com/watch?app=desktop&v=adzewZEj2Pg [Accessed 15 Mar. 2024].



---

[Undoing Changes](docs/16-oopsy-undoing-changes.md) | [Workflows](18-workflows.md)
