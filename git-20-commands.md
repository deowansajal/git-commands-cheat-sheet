# Basic 20 Git Commands

## 1. git init

Initializes a new Git repository in the current directory.

```sh
git init
```

## 2. git clone

Clones an existing Git repository from a remote location.

```sh
git clone <repository_url>
```

## 3. git status

Displays the state of the working directory and the staging area.

```sh
git status
```

## 4. git add

Adds changes in the working directory to the staging area.

```sh
git add <file_name>
# or add all changes
git add .
```

## 5. git commit

Records changes to the repository with a descriptive message.

```sh
git commit -m "Commit message"
```

## 6. git push

Uploads local repository content to a remote repository.

```sh
git push origin <branch_name>
```

## 7. git pull

Fetches and integrates changes from a remote repository to the local repository.

```sh
git pull origin <branch_name>
```

## 8. git branch

Lists, creates, or deletes branches.

```sh
# List branches
git branch
# Create a new branch
git branch <branch_name>
# Delete a branch
git branch -d <branch_name>
```

## 9. git checkout

Switches branches or restores working tree files.

```sh
# Switch to a branch
git checkout <branch_name>
# Create and switch to a new branch
git checkout -b <branch_name>
```

## 10. git merge

Merges changes from one branch into the current branch.

```sh
git merge <branch_name>
```

## 11. git fetch

Downloads objects and refs from another repository.

```sh
git fetch origin
```

## 12. git remote

Manages set of tracked repositories.

```sh
# List remote repositories
git remote -v
# Add a new remote repository
git remote add <name> <url>
# Remove a remote repository
git remote remove <name>
```

## 13. git log

Shows the commit logs.

```sh
git log
```

## 14. git reset

Resets current HEAD to the specified state.

```sh
# Soft reset (keeps changes in the working directory)
git reset --soft <commit_hash>
# Hard reset (discards changes in the working directory)
git reset --hard <commit_hash>
```

## 15. git revert

Reverts changes from a specified commit by creating a new commit.

```sh
git revert <commit_hash>
```

## 16. git stash

Temporarily saves changes that are not ready to be committed.

```sh
# Save changes
git stash
# Apply stashed changes
git stash apply
# List stashed changes
git stash list
```

## 17. git tag

Creates, lists, or deletes tags.

```sh
# Create a new tag
git tag <tag_name>
# List tags
git tag
# Delete a tag
git tag -d <tag_name>
```

## 18. git diff

Shows changes between commits, commit and working tree, etc.

```sh
# Compare working directory and staging area
git diff
# Compare staging area and last commit
git diff --staged
# Compare two commits
git diff <commit1> <commit2>
```

## 19. git rm

Removes files from the working directory and the staging area.

```sh
git rm <file_name>
```

## 20. git config

Sets configuration values for your Git installation.

```sh
# Set user name
git config --global user.name "Your Name"
# Set user email
git config --global user.email "your.email@example.com"
# Set default editor
git config --global core.editor "code --wait"
```
