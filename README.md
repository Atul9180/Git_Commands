# Git_Commands: 

## Task 1. Copying Content to Another Branch, to make new changes in main branch without affecting child branch :
This guide outlines steps to copy content from the main branch to another branch in Git.

##### Step 1: Create a New Branch and Copy Content:
```bash
# Checkout to the main branch
git checkout main

# Create and switch to a new branch (e.g., 'other-branch')
git checkout -b other-branch

# Push the new branch to the remote repository (if needed)
git push origin other-branch
```

##### Step 2: Make Changes in the Main Branch:
```bash
# Switch back to the main branch
git checkout main

# Make changes in the main branch (add, edit, delete files, etc.)
# Commit the changes
git add .
git commit -m "Updated content in main branch"
```


## Task 2. To revert the changes to the second last commit in Git, you can use the git reset command. Assuming you want to keep the changes from the most recent commit intact:

### Soft Reset (Preserving Changes):
```bash
# Check the commit history to identify the commit to which you want to reset
git log

# Reset to the commit before the last commit, preserving changes
git reset --soft HEAD~2

# Check the changes to ensure it's as expected
git status
```
###### *Note: Remember, a git reset --soft keeps changes in the staging area/index. If you want to discard changes completely, you can use --hard instead of --soft. However, be cautious as the --hard option will discard all changes irreversibly. Always ensure to review changes using git status and git diff before making any final commitments.
