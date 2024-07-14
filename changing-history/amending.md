# Git Commit Amend

### Amend is not a git command
Amend is an option in `git commit`. Not a command

### Purpose of amending
Modify last unpushed commit (will create a new commit hash)
`git commit --amend`

You can change commit message or changing committed files

#### DO NOT AMEND PUBLIC COMMIT!

### Example

Before:
```
[sora@pop-os:~/Projects/git-playground/changing-history] (main) $ git log --oneline
933f3b7 (HEAD -> main) Added test-amending
511ac46 (origin/main) Added TODO.md
51a1175 Added new note
fe61773 Added question
078753e (origin/branch-ax-remote, branch-ax-local) Added push new branch note
b64c553 Updated setup.md
b67f046 Updated setup.md
1bbc7d2 Added newlines
db7a47c Added publish new branch note
3952b62 Updated setup.md
5f5af67 Updated README.md
14ebf56 Added setup note
63cce3c Init repo
```

After:
```
[sora@pop-os:~/Projects/git-playground/changing-history] (main) $ git commit --amend -m "Added amending.md"
[main bd443a0] Added amending.md
 Date: Sun Jul 14 13:49:29 2024 +0700
 2 files changed, 12 insertions(+)
 create mode 100644 changing-history/amending.md
 create mode 100644 changing-history/test-amending
[sora@pop-os:~/Projects/git-playground/changing-history] (main) $ git log --oneline
bd443a0 (HEAD -> main) Added amending.md
511ac46 (origin/main) Added TODO.md
51a1175 Added new note
fe61773 Added question
078753e (origin/branch-ax-remote, branch-ax-local) Added push new branch note
b64c553 Updated setup.md
b67f046 Updated setup.md
1bbc7d2 Added newlines
db7a47c Added publish new branch note
3952b62 Updated setup.md
5f5af67 Updated README.md
14ebf56 Added setup note
63cce3c Init repo
```
