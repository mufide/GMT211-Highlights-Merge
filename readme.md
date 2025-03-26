## ⚠️ Important Points to Consider

### 1. README Content Requirements

For each GitHub assignment, your `README.md` file should include the following:

- A brief explanation about the assignment  
- At least one image  
- A table (if applicable)  

### 2. Adding Images Correctly

Please **use relative paths** when inserting images. This allows you to push both the image and the README file at the same time.

✅ Recommended format:
```markdown
![Git Download](/img/git-download.png)
```

❌ Not recommended (but still works):
```markdown
![Git Install](https://github.com/username/repo-name/blob/master/img/git-install.png)
Using a full GitHub URL like above requires these extra steps:
-First, push the image
-Then copy the GitHub-hosted image URL
-Finally, update your README with that URL
```
This process creates unnecessary workload.
**To keep it simple, prefer the relative path format whenever possible.**

### 3. Meaningful Commit Messages

When working on your assignments, make sure your commit messages are **clear, descriptive**, and meaningful.  
Each message should help you (and others) understand what changes were made in that commit.

Good commit messages should:
- Clearly explain what was done
- Be related to the actual changes
- Help you remember the purpose of the update later

**Note:** Your commit messages will also be reviewed during the evaluation of your assignments.

---

## Merge Process Steps

A **branch** is a copy of the main project where you can make changes without affecting the main version. It's commonly used for:
- Adding new features
- Fixing bugs
- Testing without risk

**Merge** is the process of combining changes from one branch into another — usually from a feature branch into the `main` (or `master`) branch.


### Step-by-Step: Branch & Merge

###  1. Create a New Branch
```bash
git branch yourbranchname
```

###  2. Switch to the New Branch
```bash
git checkout yourbranchname
```

###  3. Merge the Branch into main
```bash
git checkout main     #First, switch to the main branch
git pull origin main    #Then pull the latest changes from the remote
git merge yourbranchname    #Now merge your feature branch into main
git push origin main   #Finally, push the updated main to GitHub
```
