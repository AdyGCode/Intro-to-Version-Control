# Forking Over Code

So far we have gone through and practiced the concepts of:

- creating a local repository,
- adding & updating files in the staging area,
- committing files to the repository,
- creating a remote repository,
- attaching the local to the remote,
- pushing files to the remote,
- pulling files from the remote, and
- cloning an existing repository to our local machine.

Cloning is one way to work with a repository, but when you are working on an established, and predominately open source,
project, the use of a "fork" provides more control, especially for the owner(s) of the repository.

# GitHub and Forking

The concept of a fork is a GitHub feature. It basically clones the repository to another location on GitHub.

In return, GitHub maintains a link back to the original to allow collaboration on the project/repository.

## Why Fork

There are two main reasons:
1. Go your own way
2. Contribute

### Go your own way

This type of fork allows you freedom to take the project in a totally new direction.

It allows you to experiment, learn and grow.

It provides you with the opportunity to develop a new application or system based on the original, and then the ability to not look back!

Another part of this is that you still get the original project's updated code, bug fixes etc to be merged into your code at your discretion.

This type of fork gives you complete control of your project.

### Contribute

In the contribution type of fork, you are using the fork almost like a branch. 

The big thing about this is that you only need read permissions to the original repo to start working.

# Forking in the Enterprise

Remember that forking is a GitHub feature. Other Git hosting solutions may have similar features.

Forking is common practice in open source development.


# Comparing Forks v Branches

In an article by SSW in their "SSW Rules" they outline some of the fundamental differences:

|                                           | Forks                                                                                  | Branches                                                              |
| ----------------------------------------- | -------------------------------------------------------------------------------------- | --------------------------------------------------------------------- |
| **Purpose**                               | Create a separate copy of a repository for significant changes or different directions | Develop new features or fix bugs without disrupting the main codebase |
| **Relationship to the original codebase** | Completely independent repository                                                      | Linked to the original repository                                     |
| **Ownership**                             | Owned by the user who created them                                                     | Owned by the repository owner                                         |
| **Scope of changes**                      | Typically involve significant changes                                                  | Typically involve smaller changes                                     |
| **Collaboration**                         | Used to develop ideas in isolation from the main team                                  | Used to develop ideas that the main team is working on                |

> Based on SSW.Rules "Do you know when to create a fork vs a branch".
> 
  SSW.Rules. (n.d.). _Git - Do you know when to create a fork vs a branch?_ [online] Available at: https://www.ssw.com.au/rules/fork-vs-branch/ [Accessed 14 Mar. 2024].

# How to Fork

Forking is done within the GitHub Web GUI.

The basic process is:

- Find the repository you wish to fork
- Read the ReadMe and any documentation on how to fork and contribute to the repository
- Fork the repository (to your account)
- Clone the repository to your local device



# Pull Requests

A pull request is a GitHub feature (with similar features in other git hosting).

A pull request proposes the target repo pulls from a secondary repo or branch. This is in place of pushing to a target repo (“production”) or merging to a production branch.

Thus “pull request” means:
> request a pull from your branch instead of pushing to the target repo/branch

### Anatomy of a Pull Request

A pull request has the following features:
- Has a target repo/branch <=> source repo/branch
- Has a state: Open, Closed, Merged, Draft
- Presents a moving Δ between the target and source
- Contains an area to review and discuss, including in line comments
- May be a trigger for automated checks and workflows

#### When combined with Protected Branches

GitHub allows you to specify that branches with a given name pattern are protected, this means that the branch may insist on:
- A pull request before merge,
- At least X reviewers or particular reviewers before merge is permitted
- and other limitations on the request.

## How to Make a Pull Request

Imagine you created a fork or branch or both, and you think your changes are good enough for the main branch/repo... What should happen next?

There are two options:
- Merge and see
- Propose, discuss/review, then merge

### Merge and See

In “merge and see” your merge your changes and hope for the best. 

This is not as crazy as it sounds since Git is meant to provide us with fail safes... What are the fail safes Git provide you with?

But:
- You must have permissions to merge into the repo/branch
- The code may not meet quality standards and organizational requirements
- These may be “silent but deadly”...

A better option could be...

### Propose, Discuss/Review and Merge

Many people and organizations want to review proposed changes prior to merging. This is because the prospect of "bad code" becoming part of the software is not something anyone looks forward to.

The process of Propose, Review and Merge provides the following advantages:
- Enhances quality
	- The process ensures that code that gets “mainlined” has been proofed.
- Encourages collaboration
	- Any changes are not just the responsibility of the contributor of the code. 
	- Reviewers and the owners of the project also have a stake in a change.
- Improves security
	- We can have more authors than committers to the project.
	- These committers act as ‘gatekeepers’ who are the only ones allowed to merge a proposed set of a changes to given repos and branches.

## Exercise

In this repository you will find an exercise that you should download and follow. It is a single Markdown document with all the steps to practice pull requests. Download the [Pull Request Practice Read Me Markdown document](../assets/Pull-Request-Practice.md), and rename it `ReadMe.md`.

Open this file and follow the instructions.

To go with this exercise, there is an image, [collaboration.png](../assets/collaboration.png) to be downloaded and used in the exercise.

[13: Cloning](13-why-hello-dolly.md) | [15: Workflows](18-workflows.md)
