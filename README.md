
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
7. Use `git reset` + `--hard` + `HEAD^` to undo the last commit and discard all changes (both in the working directory and the staging area). Notice that `HEAD^` means the last commit, `HEAD^^` means the commit before the last commit, and so on. Or, use `git reset` + `--soft` + `HEAD^` to undo the last commit and return the changes to the staging area. Or, use `git reset` + `--mixed` + `HEAD^` to undo the last commit and return the changes to the working directory. Note: `git reset --mixed` is actually the default option for `git reset`.
8. 