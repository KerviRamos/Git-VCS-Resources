# GIT - Version Control System 
Git is a "content addressable filesystem" with a version control interface. Git is primarily known for allowing its user to collaborate in large projects and keep track of any files. This page will walk through the GIT's data model and summarize the commands available in git.

### Summary of resources 
The following resources can be found in this repository folder structure

    GIT-VCS-Resources/
    |- README.md           # Repository overview
    |
    |- keyNote/            # Git keynote presentation
    |
    |- pdfs/               # Git presentation in pdf format
    |
    |- pngs/               # reference images


## Git Data Model - Content-Addressable Filesystem Structure
How does the "content addressable filesystem works or what does it even mean? 
At its core has a unique way it stores data. Git stores data in a key-value format.

(data model will be explain here - UNDER DEVELOPMENT)

## Git Commands - Version Control Interface

#### Basics

* `git init` initializes the .git database
* `git clone <url>` downloads a remote repository to your local working space
* `git status` or `git status -s` summarizes the current state of your repo
* `git add <filename(s)>` stages files for the next commit
* `git diff <filename>` shows the difference between the staged and the modified file
* `git diff --staged` shows the difference between committed and the staged files
* `git commit -m "commit message"` creates a commit to the .git repo with a message
* `git commit -a -m "commit message"` stages the modified files and commits the files
* `git rm <filename>` removes a file
* `git mv <oldfilename> <newFilename>` renames any tracked file
* `git log --graph --decorated` shows the git history in graph format

#### Remotes

* `git remote -v`  showing your remotes repositories
* `git remote show <name>` detail metadata of remote repo
* `git remote add <name> <url>` add the remote repository with specifed name
* `git remote rename <old> <new>` renames the remote repo
* `git remote remove <name>` removes remote tracking branches and configuration settings associates with that remote
* `git pull <name>`  Fetches and merges the remote branch into your current local master branch
* `git fetch <name>` Downloads the remote repo without downloading
* `git push <RemoteName> <BranchName>` Uploads your local branch data to the remote branch. You must have write access

#### Undoing

* `git commit --amend` allows you add missing files to your commit or modified the commit message
* `git reset HEAD <filename>` unstages a file
* `git checkout --<filename>` discard changes

#### Tagging

* `git tag <tagName>` creates a lighweight tag reference
* `git tag -a <tagName> -m “message”` creates an annotated tag object
* `git tag [-l or —list]`  list all available tags 
* `git show <tagName>` shows extra tag information
* `git push origin <tagName> or —tags` uploads the tags to your remote repo
* `git tag -d <tagName>` deletes a tag on your local repository

#### Branching
(UNDER DEVELOPMENT)

#### Advanced Tools In GIT
(UNDER DEVELOPMENT)

## REFERENCES
1. [Pro Git by Scott Chacon and Ben Straub](https://git-scm.com/book/en/v2) Pro Git contains all the information you need to learn Git. A lot of the material derived in this repository comes from reading Pro Git and my personal experience using git.

2. [Oh dangit, Git!?! by Katie Sylor-Miller](https://dangitgit.com/en) Great blog/site outlining ways to get out of bad situations in git. If you have some mistakes while using git, this blog will save your life.