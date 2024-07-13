# Publish new branch

### Create new branch
1. `git branch <new branch name>` create new branch
2. `git checkout -b <new branch name>` this will create and checkout a new branch

### Switch between branches
when switch to branch it will output:

```
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
```
When switch to new branch, it doesn't show the second line because we haven't set what origin branch to track yet.

1. `git switch` new prefer way to switch between branch
2. `git checkout <branch name>`

