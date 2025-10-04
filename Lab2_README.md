# 🌩️ Cloud Computing – Lab 2  
## Git Installation & GitHub Workflow

**Name:** Saira Ejaz  
**Reg No:** 2023-BSE-057  
**Section:** 5-B  
**Subject:** Cloud Computing  
**University:** Fatima Jinnah Women University, Rawalpindi  
**Department:** Software Engineering  

---

## 📘 Lab Overview
This lab covers installation and setup of Git, GitHub repository management, branching, merging, and collaboration workflows.

---

## 🧩 Task 1: Create Private GitHub Repository
1. Log in to your GitHub account.
2. Click **New Repository** → Name it **Lab2**.
3. Set visibility to **Private**.
4. Click **Create Repository**.
5. Go to **Settings** and confirm the repository is private.
6. Take a screenshot of settings → `repo_private.png`

📸 **Screenshot:**  
`repo_private.png`

---

## ⚙️ Task 2: Connect Repository via SSH
1. Open **Git Bash**.
2. Generate SSH key:
   ```bash
   ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
   ```
3. Copy your SSH public key:
   ```bash
   cat ~/.ssh/id_rsa.pub
   ```
4. Add key to GitHub → **Settings → SSH and GPG keys → New SSH key**.
5. Test connection:
   ```bash
   ssh -T git@github.com
   ```

📸 **Screenshot:**  
`screenshot_ssh_connection.png`

---

## 👤 Task 3: Configure Git Username and Email
```bash
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
git config --list
```
📸 **Screenshot:**  
`screenshot_git_config.png`

---

## 📂 Task 4: Explore the `.git` Folder
1. In your project folder, open **Git Bash**.
2. Type:
   ```bash
   ls -a
   ```
3. Observe `.git` directory — it contains all version control data.

📸 **Screenshot:**  
`screenshot_git_folder.png`

---

## 🗂️ Task 5: Local Repository Management
1. Delete existing `.git` folder:
   ```bash
   rm -rf .git
   ```
2. Re-initialize Git:
   ```bash
   git init
   ```
3. Create README file:
   ```bash
   echo "# Lab2" > README.md
   git add README.md
   git commit -m "Initial commit"
   ```
4. Connect to GitHub:
   ```bash
   git remote add origin git@github.com:<username>/Lab2.git
   git push -u origin main
   ```

📸 **Screenshot:**  
`screenshot_repo_init.png`

---

## 📄 Task 6: File Status & Staging
1. Create a new file:
   ```bash
   echo "print('Hello Git!')" > main.py
   ```
2. Check file status:
   ```bash
   git status
   ```
3. Stage and commit:
   ```bash
   git add main.py
   git commit -m "Added main.py"
   ```

📸 **Screenshot:**  
`screenshot_git_status.png`

---

## 🌿 Task 7: Branch Creation Using GitHub GUI
1. Open **GitHub Repo → Branch Dropdown → New Branch**.
2. Name branch as `feature/gui-test`.
3. Click **Create Branch**.

📸 **Screenshot:**  
`screenshot_github_branch.png`

---

## 🌱 Task 8: Branch Creation and Push Using Git Bash
```bash
git checkout -b feature/db-connection
git push origin feature/db-connection
```

📸 **Screenshot:**  
`screenshot_git_branch_push.png`

---

## 🔀 Task 9: Branching & Merging
1. Create a new branch and switch:
   ```bash
   git checkout -b feature/add-function
   ```
2. Edit `main.py` → Add a function.
3. Commit changes:
   ```bash
   git add main.py
   git commit -m "Added function in main.py"
   ```
4. Switch to main and merge:
   ```bash
   git checkout main
   git merge feature/add-function
   git push origin main
   ```

📸 **Screenshot:**  
`screenshot_merge_main.png`

---

## 🧩 Task 10: Pull Request and Branch Review (GitHub GUI)
1. Go to **Pull Requests** tab → Click **New Pull Request**.
2. Choose branch (e.g., `feature/db-connection` → `main`).
3. Click **Create Pull Request**.
4. Review and merge it.
5. Delete branch after merge.

📸 **Screenshot:**  
`pr_created.png`  
`pr_merged.png`  
`branch_deleted.png`

---

## 🌳 Task 11: Detailed Branch Strategy (Develop/Staging)
Branch Strategy:
- `feature/*` → For development of new features.  
- `bugfix/*` → For fixing issues.  
- `develop` → Integration branch where features are merged.  
- `staging` → Pre-production testing branch.  
- `main` → Production-ready code.

Workflow:
1. Developers work on `feature/*` and `bugfix/*`.
2. Merge into `develop`.
3. Merge `develop` → `staging` for testing.
4. Merge `staging` → `main` for deployment.

📸 **Screenshots:**  
`branch_strategy.png`  
`branch_merges.png`  
`final_merge.png`

---

## 👥 Bonus Task: Simulated Team Collaboration
Example:
- Developer A: Works on `feature/login`.
- Developer B: Works on `feature/signup`.
- Both push to remote → merged into `develop`.

📸 **Screenshot:**  
`collaboration_example.png`

---

## 🧾 Task 12: Code Review Workflow
1. Create a Pull Request (PR) from a feature branch.
2. Assign reviewer on GitHub (right sidebar).
3. Reviewer approves or suggests changes.
4. Update `main.py` if needed.
5. Merge PR.
6. Delete branch after merge or keep it with reason in `REVIEW_NOTES.md`.

📸 **Screenshots:**  
`pr_assigned_reviewer.png`  
`review_approved.png`

---

## 🧹 Task 13: Branch Cleanup Best Practices
1. Delete remote branch using GitHub UI.  
2. (Optional) Verify via Git Bash:
   ```bash
   git fetch -p
   git branch -a
   ```
3. Update local repository:
   ```bash
   git checkout main
   git pull origin main
   git branch -d <branch-name>
   ```

📸 **Screenshots:**  
`remote_branch_deleted.png`  
`remote_branch_delete_cmd.png`

---

## ✅ Final Checklist
- [x] Repository is **private**  
- [x] All **branches** created and merged  
- [x] **Reviewer assigned** and PR merged  
- [x] **All screenshots** uploaded  
- [x] **README.md** (this file) uploaded to repo root  

---

## 🤝 Add Professor as Collaborator
1. Go to **Repository → Settings → Collaborators**.  
2. Click **Add People**.  
3. Enter your professor’s GitHub username (e.g., `@professor-name`).  
4. Click **Add Collaborator**.

📸 **Screenshot:**  
`collaborator_added.png`

---

## 🏁 End of Lab 2 – Git Installation and GitHub Workflow
