# Gulp Commands
<p align="center">
  <br><br>
  <img src="assets/images/gulp-logo.png" width="325" height="auto"  />
</p>


## Gulp Commands
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