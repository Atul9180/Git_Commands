# Git_Commands: 


## Task: Copying Content to Another Branch, to make new changes in main branch without affecting child branch :
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
