# Commonly used Git Commands
-------------------------------------------------------------------------------------------------------------------------------------------------------------------

Git is an incredibly powerful version control system that plays a vital role in modern software development. 
For DevOps engineers, understanding Git commands is crucial for managing source code, collaborating with teams, and ensuring smooth deployment processes.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 1. git init:
The `git init` command is used to initialize a new Git repository in a directory. 
It creates a hidden .git folder, which contains all the necessary files for version control.

### Usage:
```sh
$ git init 
```
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 2. git clone:
The `git clone` command allows you to create a local copy of a remote repository. 
It downloads the entire repository, including all branches and commit history.

### Usage:
```sh
$ git clone https://github.com/example/repository.git  
```
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 3. git add:
The `git add` command is used to add files to the staging area, preparing them for the next commit. 
You can specify individual files or use wildcards to add multiple files.

### Usage:
```sh
$ git add myfile.py
$ git add *.py
$ git add .
```
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 4. git commit:
The `git commit` command creates a new commit, saving the changes made to the files in the staging area. 
It's essential to provide a descriptive commit message to document the changes.

### Usage:
```sh
$ git commit -m "Add Comment"
```
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 5. git push:
The `git push` command is used to upload local commits to a remote repository. 
It updates the remote repository with your latest changes.

### Usage:
```sh
$ git push origin main
```
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 6. git pull:
The `git pull` command fetches the latest changes from a remote repository and automatically merges them with your local branch. 
It's commonly used to update your local repository with the latest changes.

### Usage:
```sh
$ git pull origin main 
```
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 7. git branch:
The `git branch` command allows you to manage branches within a Git repository. 
It helps you create, delete, or list branches.

### Usage:
```sh
$ git branch new-feature
$ git branch -d old-feature
$ git branch  
```
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 8. git checkout:
The `git checkout` command is used to switch between branches or restore files to a previous state. 
It helps you navigate through different versions of your code.

### Usage:
```sh
$ git checkout baranchname
$ git checkout -b baranchname
$ git checkout HEAD~1 myfile.py 
```
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 9. git merge:
The `git merge` command combines changes from different branches. 
It integrates the changes made in one branch into another.

### Usage:
```sh
$ git merge branchname 
```
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 10. git log:
The `git log` command displays a detailed history of commits. 
It provides information about the author, date, and commit message of each commit.

### Usage:
```sh
$ git log     
```
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 11. git status:
The git status command displays the state of the working directory and the staging area. 
It lets you see which changes have been staged, which haven’t, and which files aren’t being tracked by Git.

### Usage:
```sh
$ git status    
```
-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 12. git config
Define author name to be used for all commits in current repo. 
Devs commonly use --global flag to set config options for current user

### Usage:
```sh
$ git config user.name <name>
$ git config user.email <email>
```
-------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Conclusion:
Git is an indispensable tool for DevOps engineers, enabling efficient collaboration and version control in software development. By mastering these essential Git commands, will enhance your ability to manage source code and streamline deployment processes. 

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
