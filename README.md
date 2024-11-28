
# First Day to formally learn Git

Actually it is the second time, since I did it in my second year of college during my undergraduate studying. But I forgot the details, so I decided to learn it again.

## What is Git?

Git is a version control system that is used to track changes in code. It is a **distributed version control system**, which means that it allows multiple people to work on the same codebase at the same time.

## How to use Git?

1. Install Git on your computer.
2. Create a new working directory and repository on your computer. This can be done by running the command `mkdir <Create Your Directory>` and `git init` in the terminal.
3. Create a new file in the repository and add it to the staging area. This can be done by running the command `git add <File Name>` in the terminal.
4. Commit the changes to the repository. This can be done by running the command `git commit -m "Commit Message"` in the terminal.
5. Always use `git status` to check the status of your repository.
6. Use `git log` to see the history of your repository and use `git reflog` to see the history of your repository including the changes that have been undone. Notice that `git reflog` record the changing history of **HEAD** pointer.
7. Use `git reset` + `--hard` + `HEAD^` to undo the last commit and discard all changes (both in the working directory and the staging area). Notice that `HEAD^` means the last commit, `HEAD^^` means the commit before the last commit, and so on. Or, use `git reset` + `--soft` + `HEAD^` to undo the last commit and return the changes of present version the staging area. Or, use `git reset` + `--mixed` + `HEAD^` to undo the last commit and return the changes of present version to the working directory. Note: `git reset --mixed` is actually the default option for `git reset`.
8. Use `git checkout` + `HEAD` to return to the last commit. Use `git checkout` + `--` + `<File Name>` to discard the changes of the file in the working directory. Use `git checkout` + `<Branch Name>` to switch to the specified branch.
9. Use `git branch` to list all the branches in the repository. Use `git branch` + `<Branch Name>` to create a new branch. Use `git branch` + `-d` + `<Branch Name>` to delete the specified branch. Use `git merge` + `<Branch Name>` to merge the specified branch into the current branch.
10. Use `git push` to push the changes to the remote repository.
11. Use `git pull` to pull the changes from the remote repository.
12. Use `git clone` + `<Repository URL>` to clone the repository from the remote server.
13. Use `git remote` to list all the remote repositories. 
    - Use `git remote` + `-v` to list all the remote repositories with their URL.
    - Use `git remote` + `add` + `<Remote Name>` + `<Repository URL>` to add a new remote repository.
    - Use `git remote` + `rm` + `<Remote Name>` to remove a remote repository.
    - Use `git remote` + `rename` + `<Old Name>` + `<New Name>` to rename a remote repository.
    - Use `git remote` + `set-url` + `<Remote Name>` + `<New URL>` to set the URL of a remote repository.
    - Use `git remote` + `show` + `<Remote Name>` to show the information of a remote repository.

## Core concepts of Git

1. **Repository**: A repository is a directory that contains all the files and metadata needed to track changes to the files.
2. **Working Directory**: The working directory is the directory that contains the files that you are currently working on.
3. **Staging Area**: The staging area is a temporary area where you can add changes to the files before committing them to the repository.
