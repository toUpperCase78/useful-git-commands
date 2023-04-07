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



## Previously...

I had performed a demonstration to push files from my local repository to this remote repo here.

It worked by using `git push`, including two other git commands beforehand: `remote` and `branch`

These commands had been entered inside git bash while in my local directory:

* `git remote add origin <clone-url>`
* `git branch -M main`
* `git push -u origin main`
