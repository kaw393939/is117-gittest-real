# Question 1: What does `git status` do and when would you use it?

## Answer

`git status` shows the current state of your working directory and staging area. It tells you which files have been modified, which are staged for commit, and which are untracked.

You would use it:
- Before making a commit to see what changes will be included
- To check if you're on the right branch
- To see if there are any uncommitted changes
- After pulling to see if there are any conflicts

## Example

```bash
$ git status
On branch main
Changes not staged for commit:
  modified:   README.md

Untracked files:
  newfile.txt
```
