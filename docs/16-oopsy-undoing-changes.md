# Undoing Changes

You've made an error in your commits, merges or such ... do not worry, it happens to the best of us.

Remember that Git stores EVERYTHING.

The problem is that this isn't always the best thing.

We will make errors such as:
- Accidently add a file you did not want to add.
- Make a commit you didn’t intend to commit (too soon, wrong branch, etc).
- Make a commit and decide you want to change it or its commit message.
- Push a change you didn’t mean to push.
- Make updates to your working copy you want to remove!

Making these errors will happen at some point.

## We will mend it, we will fix it...

Anything can be fixed but the difficulty level does rise pretty quickly. Some may say exponentially.

In general, there are two strategies:
- Revert changes by creating a new commit
- Reset changes by removing them from history

Each has their respective advantages.

|                         | Git Revert                                                   | Git Reset                                                                        |
| ----------------------- | ------------------------------------------------------------ | -------------------------------------------------------------------------------- |
| **Operation**           | Creates a new commit that undoes changes                     | Moves the branch pointer to a previous commit                                    |
| **Commit History**      | Preserves the original commit history                        | Modifies the commit history                                                      |
| **Branch State**        | Updates the branch with a new commit                         | Moves the branch pointer to a different commit                                   |
| **Working Directory**   | Does not modify the working directory                        | Can optionally modify the working directory                                      |
| **Collaboration**       | Safe for shared repositories, as it creates a new commit     | Potentially dangerous for shared repositories, as it rewrites the commit history |
| **Use Cases**           | Undoing commits, fixing mistakes, reverting changes          | Discarding local commits, cleaning up history, resetting to a previous state     |
| **Remote Repositories** | Suitable for reverting changes pushed to remote repositories | Not suitable for resetting changes pushed to remote repositories                 |

## Warning: Reset Danger

WARNING: resets are hazardous!

You run the risk of:
- Losing work.
- Misaligning the commit history (after push).

## Git Reset

<iframe width="560" height="315" src="https://www.youtube.com/embed/iEgCj-d-G5U?si=oHntqxD_L65V_k-E" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Git Revert

<iframe width="560" height="315" src="https://www.youtube.com/embed/XJqQPNudPSY?si=RapMB35X1eefT6N4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

# References

A Shot of Code (2023). _Git Reset Visualized_. [online] www.youtube.com. Available at: https://www.youtube.com/watch?v=iEgCj-d-G5U&list=PLvVKmViR0Z7aKwZjgICrjp0wUYMF_IpGX&index=14 [Accessed 15 Mar. 2024].

A shot of code (2023). _Git Revert - Visualised_. [online] www.youtube.com. Available at: https://www.youtube.com/watch?v=XJqQPNudPSY&list=PLvVKmViR0Z7aKwZjgICrjp0wUYMF_IpGX&index=15 [Accessed 15 Mar. 2024].


[Diffs](14-diffs.md) | [Stashing](17-stashing.md)
