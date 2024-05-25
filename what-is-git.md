# What is Git?

Git is a distributed version control system designed to handle everything from small to very large projects with speed and efficiency. 
It is free and open-source software originally created by Linus Torvalds in 2005.

## Key Features of Git

- **Distributed System**: Every developer has a complete copy of the entire repository, including the full history of changes.
- **Speed**: Git is fast. Performing actions such as commits, diffs, and merges can be done quickly.
- **Scalability**: Git can handle projects of any size, from a few files to large codebases with millions of lines of code.
- **Branching and Merging**: Git makes branching and merging straightforward and helps in parallel development workflows.
- **Data Integrity**: Git ensures the integrity of your data using a combination of SHA-1 hashes to track changes.

## Why Use Git?

- **Version Control**: Keep track of every change to your codebase, who made the change, and when it was made.
- **Collaboration**: Multiple developers can work on the same project simultaneously without interfering with each other.
- **Backup**: Every clone of the repository is a full backup, reducing the risk of data loss.
- **Reversibility**: Easily revert to previous states of the codebase if something goes wrong.

## Basic Concepts

- **Repository**: A Git repository is a storage space where your project lives. It tracks and saves the complete history of your changes.
- **Commit**: A commit is a snapshot of your repository at a specific point in time. Each commit has a unique ID.
- **Branch**: A branch is a separate line of development. You can create branches to work on new features without affecting the main codebase.
- **Merge**: Merging is the process of combining the changes from different branches into one.

## Deep into the git workflow.

There are three core areas to git. These are the Working Tree, the Staging Area (also known as Index), and the Local Repository. 
When working in a git repository, files and modifications will travel from the Working Tree to the Staging Area and finish at the Local Repository. 
Thus we will talk about these three areas in that order.

### The Working Tree
The Working Tree is the area where you are currently working. It is where your files live. 
This area is also known as the “untracked” area of git. 
Any changes to files will be marked and seen in the Working Tree. 
Here if you make changes and do not explicitly save them to git, you will lose the changes made to your files. 
This loss of changes occurs because git is not aware of the files or changes in the Working Tree until you tell it to pay attention to them. 
If you make changes to files in your working tree git will recognize that they are modified, but until you tell git “Hey pay attention to these files,” it won’t save anything that goes on in them.

Run the command ```git status```. 

This command will show you two things: The files in your Working Tree and the files in your Staging Area. 
It will look something like the image below if you don’t have anything in your Staging Area.

![image](https://github.com/AmalSunny992/gitcommands/assets/169422802/9ce7a1b6-e04f-4592-9658-b8e6dc954825)

### The Staging Area (Index):
The Staging Area is when git starts tracking and saving changes that occur in files. 
These saved changes reflect in the .git directory. That is about it when it comes to the Staging Area. 
You tell git that I want to track these specific files, then git says okay and moves them from you Working Tree to the Staging Area and says “Cool, I know about this file in its entirety.” 
However, if you make any more additional changes after adding a file to the Staging Area, git will not know about those specific changes until you tell it to see them. 
You explicitly have to tell git to notice the edits in your files.

Run the command ``` git status ``` to see what is in your Staging Area. It will look something like the image below.

![image](https://github.com/AmalSunny992/gitcommands/assets/169422802/b79e0092-8cca-40e9-aa57-35e70339404e)

Running the command ``` git add #filename# ``` will add a specific file to the Staging Area from your Working Tree. 
If you want to add everything from the Working Tree, then run the command ``` git add . ``` . The . operator is a wildcard meaning all files.

### The Local Repository:
The Local Repository is everything in your .git directory. 
Mainly what you will see in your Local Repository are all of your checkpoints or commits. 
It is the area that saves everything (so don’t delete it). That’s it.

The git command ``` git commit ``` takes all changes in the Staging Area, wraps them together and puts them in your Local Repository. 
A commit is simply a checkpoint telling git to track all changes that have occurred up to this point using our last commit as a comparison. 
After committing, your Staging Area will be empty.

### So what commands should be used frequently?


Using ``` git log ``` command brings up a log of all previous checkpoints in the repository.

Using ``` git status --long ``` allows to get a comprehensive list of what is in the Working Tree and Staging Area. 
It lets you to know what files have been added, modified, and which files git is tracking.

``` git diff ``` command shows you the code differences between a file in the Staging Area and the edits made to that file that currently exist in the Working Tree. 

``` git status ``` and ``` git diff ``` should frequently be used as they give you information about your current working state and what git is aware of. 
They allow you to see what changes have occurred since your last checkpoint and are what I use most often to guide myself to atomic commits.

## Learning More

To learn more about Git, you can refer to the following resources:
- [Official Git Documentation](https://git-scm.com/doc)
- [Pro Git Book](https://git-scm.com/book/en/v2)
- [Git Cheat Sheet](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet)
