# useful-git-commands

I've seen lots of cheat sheets from various sources ion the Internet, presents many commands related to Git version control. Here are the most useful ones below:

_Also uploaded Git Cheat Sheets images that explain the commands with some visuals. Be sure to check them out above!_

### CREATE

Clone an existing repository: `$ git clone <github_website_ending_with_git>`

Create a new local repository: `$ git init`

### LOCAL CHANGES

See the latest status in your working directory: `$ git status`

See changes to tracked files: `$ git diff`

Add all current changes to the next commit: `$ git add .`

Add some changes in file to the next commit: `$ git add -p <file>`

Commit all local changes in tracked files: `$ git commit -a`

Commit previously staged changes: `$ git commit`

Change the last commit: `$ git commit --amend`

### COMMIT HISTORY

Show all commits, starting with the newest on top: `$ git log`

Show changes over time for a specific file: `$ git log -p <file>`

Who changed what and when in file: `$ git blame <file>`

### BRANCHES & TAGS

List all existing branches: `$ git branch`

Switch to the branch: `$ git checkout <branch>`

Create a new branch based on your current HEAD: `$ git branch <new_branch>`

Create a new tracking branch based on a remote branch: `$ git checkout --track <remote/branch>` 

Delete a local branch: `$ git branch -d <branch>`

Mark the current commit with a tag: `$ git tag <tag_name>`

### UPDATE & PUBLISH

List all currently configured remotes: `$ git remote -v`

Show information about a remote: `$ git remote show <remote>`

Add new remote repository, named 'remote': `$ git remote add <shortname> <url>`

Download all changes from 'remote', but don't integrate into HEAD: `$ git fetch <remote>`

Download changes and directly merge/integrate into HEAD: `$ git pull <remote> <branch>`

Publish local changes on a remote: `$ git push <remote> <branch>`

Delete a branch on the remote: `$ git branch -dr <remote/branch>`

Publish your tags: `$ git push --tags`

### MERGE & REBASE

Merge branch into your current HEAD: `$ git merge <branch>`

Rebase your current HEAD onto branch: `$ git rebase <branch>`

Abort a rebase: `$ git rebase --abort`

Continue a rebase after resolving conflicts: `$ git rebase --continue`

User your configured merge tool to solve conflicts: `$ git mergetool`

Use your editor to manually solve conflicts and (after resolving) mark file as resolved: `$ git add <resolved_file>`, `$ git rm <resolved_file>`

### UNDO

Discard all local changes in your working directory: `$ git reset --hard HEAD`

Discard local changes in a specific file: `$ git checkout HEAD <file>`

Revet a commit (by producing a new commit with contrary changes): `$ git revert <commit>`

Reset your HEAD pointer to a previous commit and discard all changes since then: `$ git reset --hard <commit>`

And preserve all changes as unstaged changes: `$ git reset <commit>`

And preserve uncommitted local changes: `$ git reset --keep <commit>`

## Previously...

I had performed a demonstration to push files from my local repository to this remote repo here.

It worked by using `git push`, including two other git commands beforehand: `remote` and `branch`

These commands had been entered inside git bash while in my local directory:

* `git remote add origin <clone-url>`
* `git branch -M main`
* `git push -u origin main`
