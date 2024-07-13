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

### Setup stream or set remote tracking branch
Similar to pushing new project to remote repo, When we do `git push -u origin <branch name>`,\
We are setting remote tracking branch. So when we create new branch we have to do the same thing.

Example.
```
git checkout -b branch-a
git push -u origin branch-a
```
This will check you out to new branch named 'branch-a'.\
The latter command will set remote tracking of local branch 'branch-a' to remote origin named 'branch-a' also.

