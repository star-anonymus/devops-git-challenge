# Proof of Work - DevOps Git Challenge

**Student:** Shehryar Ahmed
**Repository:** https://github.com/star-anonymus/devops-git-challenge

## 1. Commit History (git log --oneline)

```
330ee79 (HEAD -> main, origin/main) Merge pull request #1 from star-anonymus/development
18dd302 (origin/development, development) Remove overleft conflict markers from deploy.sh
217e5c6 Resolve merge conflict between development and staging
623028a (origin/staging, staging) Update deploy script for staging environment
a82fef4 Update deploy script for development environment
72bc72a Convert deploy.sh and REAMME.md to pplain text
e3e7fd5 Initial commit: add deploy.sh and README.md
```

## 2. Reflection Questions

### Q1: Difference between Git and GitHub
Git is the version control tool that runs on my own computer and keeps track of every change I make to my files. It works completely offline, so I can commit, create branches and check history without internet. GitHub is a cloud platform that hosts Git repositories online. It lets me back up my work, share it with others and collaborate through features like Pull Requests. In this activity I used Git in the terminal for commits, stashing and merging, and GitHub to open and merge the Pull Request.

### Q2: Working Directory, Staging Area and Local Repository
The working directory is the folder where I actually edit files, like when I changed deploy.sh. When I run git add, those changes move to the staging area, which works like a waiting room where I choose exactly what goes into the next commit. When I run git commit, everything in the staging area is saved permanently in the local repository (the .git folder) as a snapshot with a message. This three-step flow gives me control, so I do not have to commit every change at once.

### Q3: git stash pop vs git stash apply
Both commands bring stashed changes back into the working directory. git stash pop restores the changes and then removes that stash from the stash list. git stash apply restores the changes but keeps the stash saved, so it can be applied again on another branch if needed. In this activity I used git stash pop because I only needed my development changes back once.

### Q4: git fetch vs git pull
git fetch downloads the latest changes from the remote repository but does not change my local files or branches. It is a safe way to see what has changed before deciding what to do. git pull does a fetch and then immediately merges those changes into my current branch. In Task 5, I used git pull after merging the Pull Request on GitHub to bring the merged code into my local main branch.
