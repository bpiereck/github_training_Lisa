# Command lists

`git init` : initialize the local repository

`git status` : check in what conceptual area your file is

Uncomitted: File is in the staging area
Unstaged: Git has an old version but there are new changes
Untracked: Completely new file, never seen it before

Good pratice: check the status of your file before every commit

- basic routine

`git add <filename>` : this will add the file to the staging area. Area to organize your "library" structure.

`git commit -m "meaningful commit message"` : this will create a version in my timeline

- time travelling

`git log <filename>`: to get a timeline of all the commits

`git log -n 3 --abbrev-commit`: will give only the last 3 commits with the smallest commit_hash as possible. 

`git diff <commit_hash1> <commit_hash2>`: to see the changes between 2 commits. Always start with the oldest commit and then the newest one.

`git show <commit_hash1>` or `git show <commit_hash1> <commit_hash2>` : show the changes that were made in a chosen commit

- Go from local to remote

`git remote add origin <ssh-address>`: this will create a bridge between the local and the remote repositories

`git push`: will send all the commits to the remote repository

On the first time you try to push you might get the error message: 

```
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.
```
`git pull`: to update from remote to local with changes made by my collaborators or directly on the remote repository

- Accidents

After deletion of a local repository:
`git clone <remote_repository_ssh_address>`

After committing an unwanted version:
`git revert <commit_hash_of_the_unwanted_version>`

- Branches

To create a new branch: \
`git branch <name_of_branch>`

To move inside the new branch: \
`git checkout <name_of_branch>`

To create a new branch and move inside directly:\
`git checkout -b <name_of_branch>`

To push to the new branch: \
`git push --set-upstream origin <name_of_branch>`

To see all the branches (also the remote ones):\
`git branch --all` or `git branch --a`

To see all the local branches:\
`git branch --list` or `git branch -l`

- Detached head

`git checkout <commit_hash>`: will create a detached head with a past version of your code

`git switch -c <new_branch>`: will attach the detached head as a new branch

- Merging branches

`git merge <name_of_the_branch_you_want_to_merge_with_main>`: this will merge your branch into the main (don't forget to checkout to the main before you merge). Resolve the conflits in TextEditor (like Visual Studio Code) and then add and commit, The merge will then be automatic.

- Tagging

`git tag <name>`: name a commit to mark a release/good state
`git push --tags`: you have to use this command otherwise the tags are not added to GitHub

