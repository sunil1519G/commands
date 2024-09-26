# Git Commands

A comprehensive guide to essential Git commands for managing repositories.

## Table of Contents
- [Basic Commands](#basic-commands)
- [Branching](#branching)
- [Reset and Revert](#reset-and-revert)
- [Logs](#logs)

### Basic Commands
1. **Add specific files to staging**:
    ```bash
    git add <filename>
    ```

2. **Add all files to staging**:
    ```bash
    git add --all
    ```

3. **Commit changes with a message**:
    ```bash
    git commit -m "message"
    ```

4. **Add and Commit changes with a message**:
    ```bash
    git commit -am "message"
    ```

5. **Rename the last commit message**:
    ```bash
    git commit --amend
    ```
   
6. **Push changes to remote**:
    ```bash
    git push
    ```
   
7. **Pull changes from remote**:
    ```bash
    git pull
    ```

### Branching
1. **Switch to another branch**:
    ```bash
    git checkout <branch> OR git switch <branch>
    ```

2. **Create and switch to a new branch**:
    ```bash
    git checkout -b <branch-name>
    ```

3. **Delete a local branch**:
    ```bash
    git branch -D <branch_name>
    ```

### Reset and Revert
1. **Undo the last commit**:
    ```bash
    git reset HEAD~1
    ```

2. **Revert changes with a new commit**:
    ```bash
    git revert <commit-hash>
    ```

3. **Unstaged the staged files**:
    ```bash
    git reset <filename>
    ```

4. **Undo commit and keep staged changes [last 1 commit]**:
    ```bash
    git reset --soft HEAD~1
    ```

5. **Undo commit and remove all changes [last 1 commit]**:
    ```bash
    git reset --hard HEAD~1
    ```

6. **Goto that specific commit**:
    ```bash
    git reset --hard <commit-id>
    ```

### Logs
1. **View commit logs**:
    ```bash
    git log
    ```

