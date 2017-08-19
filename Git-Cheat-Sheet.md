# Git & Github Commands
<p align="center">
  <br><br>
  <img src="assets/images/git-logo.png" width="195" height="auto" style="margin-right:50px">
  <img src="assets/images/github-logo.png" width="325" height="auto"  />
</p>


## Git Commands
### Setup

|Git Command|Description|
|:----------|:----------|
|`$ git config --global user.name "[name]"`|Set your username for all Git actions|
|`$ git config --global user.email "[email]"`|Set your email for all Git actions|
|`$ git config --list`|Lists all of the config values|

### Getting Started

First go to GitHub and add a new repository.

Inside the terminal, locate to the folder you would like to start tracking

|Git Command|Description|
|:----------|:----------|
|`$ git init`|Start tracking / initialise a repository from existing code|
|`$ rm -rf .git`|Stop tracking a repository|
|`$ touch .gitignore`|Creates a .ignore file of file extensions to ignore*|
|`$ git remote add origin [GitHub repo url]`|Creates remote repository pointing to GitHub**|

*Do this first, go to the editor and edit the .gitignore file, and add in .DS_Store plus anything else
**Only needs to be done once at the start of the process

A couple more useful remote commands:

|Git Command|Description|
|:----------|:----------|
|`$ git remote set-url origin [GitHub repo url] `|Change remote repository URL|
|`$ git remote -v`|Shows name and URL of remote repository|



### General Git Commands

|Git Command|Description|
|:----------|:----------|
|`$ git status`|Provides info on files that have been amended|
|`$ git add -A`|Adds all new, amended and deleted files to the staging area|
|`$ git add [filename]`|Adds a specific amended file to the staging area|
|`$ git reset `|Removes all amended files from the staging area|
|`$ git reset [filename]`|Removes a specific amended file from the staging area|
|`$ git commit -m "[comment]"`|Commits the amended files and adds a message|
|`$ git log"`|Shows a log of the commits|
|`$ git push origin master"`|Pushes changes to the 'master' branch|
|`$ git branch -a`| Lists all of the branches in the repository and locally|

### Branching

|Git Command|Description|
|:----------|:----------|
|`$ git branch [branch name]`|Creates a branch|
|`$ git checkout [branch name]`|Switch to selected branch|
|`$ git checkout -b [branch name]`|Creates a new branch and switches to it|
|`$ git branch`|Lists branches in working repository|
|`$ git push -u origin [branch name]`|Pushes changes from this branch to the repository|


Once all changes to the working branch are completed and commited, and the changes are ready to go live, change to the master branch.

|Git Command|Description|
|:----------|:----------|
|`$ git pull origin master`|Pulls all changes from repository to the master branch|
|`$ git merge [branch name]`|Pulls all changes from the working branch to the master branch|

Then push all changes to origin master

When the branch is no longer needed, you can delete it.

|Git Command|Description|
|:----------|:----------|
|`$ git branch -d [branch name]`|Deletes a branch locally|
|`$ git push origin --delete [branch name]`|Deletes a branch from repository|

### Other Git Commands (not used as much)

|Git Command|Description|
|:----------|:----------|
|`$ git diff`|Displays changes made to the code|
|`$ git fetch origin [branch name]`|Gets latest changes from repository, does not merge with branch|
|`$ git clone [GitHub repo url] .`|Clones a repository to project folder|