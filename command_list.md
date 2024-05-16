# Command lists

`git init` : initialize the local repository

`git status` : check in what conceptual area your file is

Uncomitted: File is in the staging area
Unstaged: Git has an old version but there are new changes
Untracked: Completely new file, never seen it before

Good pratice: check the status of your file before every commit

`git log <filename>`: to get a timeline of all the commits

`git log -n 3 --abbrev-commit`: will give only the last 3 commits with the smallest commit_hash as possible. 

`git diff <commit_hash1> <commit_hash2>`: to see the changes between 2 commits. Always start with the oldest commit and then the newest one.

`git show <commit_hash1>` or `git show <commit_hash1> <commit_hash2>` : show the changes that were made in a chosen commit

- basic routine

`git add <filename>` : this will add the file to the staging area. Area to organize your "library" structure.

`git commit -m "meaningful commit message"` : this will create a version in my timeline



`
