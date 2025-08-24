| **Author :** | Ali Raza                    |
|--------------|-----------------------------|
| **Course :** | MLOps                       |
| **Module :** | Git and GitHub              |
| **Email :**  | sahilir21727@gmail.com      |

---

# 🚀 **Git and Github**
- install git in laptop other than C derive
- then open vs code terminal and config by followiing code  
    - git config --global user.name ""
    - git config --global user.email ""
- Add Github to your local PC
    - git clone github link 
    - git status
    - git pull origin main      # add any change you made in github  
- Add your local project to the Github
    - git init                  # to incorporate git in folder
    - Remove-Item -Recurse -Force .git              # disconnect git from github
    - create repositor in github with same name of your project and without .rmd file
    - git add .
    - git commit -m "first commit"
    - git remote add origin github link          # connect
    - git branch
    - git remote --v
    - git push -u origin main       # first time
    - git push command              # use onward
---

## 🔁 **To log out Git from Github**
git config --global --unset user.name   \
git config --global --unset user.email
- Search for Credential Manager in Windows Start
- Open Windows Credentials
- Find anything like git:https://github.com
- Click and remove/delete it
---

## 🔁 **GitHub Access Types – Short Guide**
### 1. Fork → Clone → Change → Push
- ✅ Changes go to **their GitHub fork**
- ❌ Your repo is not affected
- ✅ They can open a **pull request** to suggest changes

### 2. Just Clone (No Fork)
- ✅ Gets a **local copy** of your code
- ❌ Cannot push or create pull request
- ❌ Changes stay only on their computer

### 3. Add as Collaborator
- ✅ Clone your repo
- ✅ Push changes directly OR
- ✅ Pull request required if **branch is protected**
---

## 🔁 **Git Feature Branch Workflow**
This guide walks through creating a feature branch, making changes, pushing to GitHub, opening a pull request, and pulling merged code.

### 📌 Git Script  
``` bash
# Step 1: Create and switch to a new feature branch
git checkout -b feature/my-feature

# Step 2: Stage all changes
git add .

# Step 3: Commit the changes
git commit -m "Add: My feature implementation"

# Step 4: Push the feature branch to GitHub
git push origin feature/my-feature

# 👉 Go to GitHub and open a Pull Request:
#    https://github.com/your-username/your-repo/branches
#    Click “Compare & pull request” next to your branch

# Step 5: (Optional) Pull the latest changes from main after merge
git checkout main
git pull origin main
```
---

## 🔁 **General commands**
### Create a new branch and switch to it
git checkout -b feature/my-feature

### Switch to an existing branch
git checkout main

### Rename current branch
git branch -m new-branch-name

### Rename a specific branch (not checked out)
git branch -m old-branch-name new-branch-name

### Delete a local branch
git branch -d feature/old-feature                   # Use -D to force delete 

### Delete a remote branch
git push origin --delete feature/old-feature


