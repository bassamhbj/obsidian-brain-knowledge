## Add .gitignore to an existing repo
1. Add `.gitignore` file
2. Execute the following commands
```
git rm -r --cached .
git add .
git commit -m "Add .gitignore"
git push origin
```

### Set user and email for a repo
1. Execute the following commands
```
git config user.name "<user_name>"
git config user.email "<user_email>"
```

### Checkout remote branch
1. Execute the following commands
```
# Add remote branch to local repo
git fetch origin <branch_name>

# Confirm the branch is being added
git branch -r
→ Expected result: origin/<branch_name>

# Switch branch
git checkout <branch_name>
```

### Create/Pop Stash
1. Create stash
```
git stash -u
```

2. Pop stash
```
git stash pop
```