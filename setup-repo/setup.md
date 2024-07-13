# Setup Repository

1. `git init` you might want to change branch name to something else.\
Default setting set to `master` as default.\
Use `git branch -m <new name>` to rename branch\
2. Add some files to working directory (this is mandatory or it won't push project to remote repo)
3. `git add <file>` Add file to staging area
4. `git remote add <remote repo url>` to add remote repo telling git to track origin (original repo) from this remote server (use ssh link if you decide to push code via command line).\
After this you can use `git remote -v (short for verbose)` for viewing what remote server git is tracking from.
5. `git push -u origin main` publish branch and telling git to set local branch to track origin branch name 'main' (`-u` = `--set-upstream` = `--tracking`, the first one is confusing and will be deplicate so just use the latter).\
After this you can use `git branch -vv` to view what local branch track what origin branch.\
`* main 63cce3c [origin/main] Init repo`\
example output of the command.\
Left most is the name of local branch in this case it's 'main'.\
Remote tracking branch is in square bracket which is `[origin/main]`
