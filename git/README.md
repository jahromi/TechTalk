# Version Control Systems and Git

In this document we briefly review the version control history and after that we review the git and remote repository services (Github is particular)

## Version control history
1. **Stand-alone and file-focused**
    - SCCS, 1972, Unix Only
    - RCS, 1982, cross-platform, text only

    ![Stand-alone and file-focused](https://git-scm.com/book/en/v2/images/local.png)
2. **Centralized**
    - CVS, 1986, first central reoisitory, file-focused
    - Perforce, 1995
    - Subversion, 2000, track directory structure
    - Microsoft Team Foundation Server, 2010

    ![Centralized](https://git-scm.com/book/en/v2/images/centralized.png)
3. **Distributed**
    - Git, 2005, created by Linus Torvalds after the change to the BitKeeper policy
    - Mercurial, 2005, same as Git created to respond to the change in BitKeeper

    ![Distributed](https://git-scm.com/book/en/v2/images/distributed.png)

Linus Torvalds wanted a distributed system that he could use like BitKeeper, but none of the available free systems met his needs. Torvalds cited an example of a source-control management system needing 30 seconds to apply a patch and update all associated metadata, and noted that this would not scale to the needs of Linux kernel development, where synchronizing with fellow maintainers could require 250 such actions at once. For his design criterion, he specified that patching should take no more than three seconds, and added three more points:


1. Take Concurrent Versions System (CVS) as an example of what not to do; if in doubt, make the exact opposite decision.
2. Support a distributed, BitKeeper-like workflow.
3. Include very strong safeguards against corruption, either accidental or malicious.

As of 2018, almost 90% of the 74,000 developers surveyed by Stack Overflow prefer to use Git for version control. Git dominates all other version control systems and adoption is up almost 20% from 2017 according to the survey.

## Let's start with Git

### Git three stages
Git has three main states that your files can reside in: modified, staged, and committed:

* Modified means that you have changed the file but have not committed it to your database yet.
* Staged means that you have marked a modified file in its current version to go into your next commit snapshot.
* Committed means that the data is safely stored in your local database.

![Git three stages](https://git-scm.com/book/en/v2/images/areas.png)

### The Command Line
There are a lot of different ways to use Git. There are the original command-line tools, and there are many graphical user interfaces of varying capabilities. For this book, we will be using Git on the command line. For one, the command line is the only place you can run all Git commands — most of the GUIs implement only a partial subset of Git functionality for simplicity. If you know how to run the command-line version, you can probably also figure out how to run the GUI version, while the opposite is not necessarily true. Also, while your choice of graphical client is a matter of personal taste, all users will have the command-line tools installed and available.





### Basic Git commands
To use Git, developers use specific commands to copy, create, change, and combine code. These commands can be executed directly from the command line or by using an application like GitHub Desktop or Git Kraken. Here are some common commands for using Git:

* `git init` initializes a brand new Git repository and begins tracking an existing directory. It adds a hidden subfolder within the existing directory that houses the internal data structure required for version control.
* `git clone` creates a local copy of a project that already exists remotely. The clone includes all the project’s files, history, and branches.
* `git add` stages a change. Git tracks changes to a developer’s codebase, but it’s necessary to stage and take a snapshot of the changes to include them in the project’s history. This command performs staging, the first part of that two-step process. Any changes that are staged will become a part of the next snapshot and a part of the project’s history. Staging and committing separately gives developers complete control over the history of their project without changing how they code and work.
* `git commit` saves the snapshot to the project history and completes the change-tracking process. In short, a commit functions like taking a photo. Anything that’s been staged with git add will become a part of the snapshot with git commit.
* `git status` shows the status of changes as untracked, modified, or staged.
* `git branch` shows the branches being worked on locally.
* `git merge` merges lines of development together. This command is typically used to combine changes made on two distinct branches. For example, a developer would merge when they want to combine changes from a feature branch into the main branch for deployment.
* `git pull` updates the local line of development with updates from its remote counterpart. Developers use this command if a teammate has made commits to a branch on a remote, and they would like to reflect those changes in their local environment.
* `git push` updates the remote repository with any commits made locally to a branch.

Learn more from a full reference guide to Git commands.

## More Contents
### To read
1. [Getting Started - About Version Control](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)
2. [The entire Pro Git book, written by Scott Chacon and Ben Straub](https://git-scm.com/book/en/v2)
### To watch
1. [Tech Talk: Linus Torvalds on git](https://www.youtube.com/watch?v=4XpnKHJAok8)
### Cheat Sheets
1. [Git cheat sheet by Bitbucket](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet)
2. [Git cheat sheet by GitHub (1)](https://training.github.com/downloads/github-git-cheat-sheet.pdf)
3. [Git cheat sheet by GitHub (2)](https://education.github.com/git-cheat-sheet-education.pdf)
