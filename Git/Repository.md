---
id: "Repository"
aliases:
  - "Add remote repository"
tags:
  - "git"
  - "repository"
---

<!--toc:start-->
- [Add remote repository](#add-remote-repository)
- [Branch](#branch)
<!--toc:end-->

## Add remote repository
```git
git remote add origin git@github.com:...
```
`origin` is the name of the repository 
Check remote repository settings:
```git
git remote -v
```
Before push to remote repository, make sure the branch name is the same.

## Branch
find all the branch
```git
git branch -a
```
find all the branch on remote repository
```git
git remote -r 
```
Rename
```git
git branch -m oldBranchName newBranchName
```

