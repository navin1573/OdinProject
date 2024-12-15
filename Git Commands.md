
# Git Commands Quick Reference

## Setup
1. **Check Git version:** `git --version`  
2. **Set default branch to main:**  
   `git config --global init.defaultBranch main`

---

## Create a Repository on GitHub
1. Navigate to GitHub, click **"+"** → **"New repository"**.  
2. Name the repository **git_test** and check **"Add a README file"**.  
3. Click **"Create repository"**.  
4. Copy the SSH URL by clicking the green **"Code"** button and selecting **SSH**.

---

## Clone Repository Locally
1. Create a directory for repositories:  
   ```bash
   mkdir ~/repos
   cd ~/repos
```

2. Clone the repository:
    
    ```bash
    git clone git@github.com:USER-NAME/git_test.git
    ```
    
3. Verify the remote URL:
    
    ```bash
    cd git_test
    git remote -v
    ```
    

---

## Basic Git Workflow

1. **Create a new file:**
    
    ```bash
    touch hello_world.txt
    ```
    
2. **Check status:**
    
    ```bash
    git status
    ```
    
3. **Add file to staging:**
    
    ```bash
    git add hello_world.txt
    ```
    
4. **Commit changes:**
    
    ```bash
    git commit -m "Add hello_world.txt"
    ```
    
5. **View commit log:**
    
    ```bash
    git log
    ```
    

---

## Modify Files

1. **Edit `README.md` and save changes.**
2. **Check status:**
    
    ```bash
    git status
    ```
    
3. **Stage the file:**
    
    ```bash
    git add README.md
    ```
    
4. **Stage all changes:**
    
    ```bash
    git add .
    ```
    
5. **Commit staged changes:**
    
    ```bash
    git commit -m "Edit README.md and hello_world.txt"
    ```
    
6. **View updated commit log:**
    
    ```bash
    git log
    ```
    

---

## Push to GitHub

1. **Push changes to remote repository:**
    
    ```bash
    git push origin main
    ```
    
2. **Verify status:**
    
    ```bash
    git status
    ```
    

---

## Final Check

- Refresh your GitHub repository page to verify files are updated.