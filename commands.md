# Git Commands

## 1. Initialization
- **Create a new Git repository**:
  
  `git init`

## 2. Configuration
- **Set global username**:
  
  `git config --global user.name "aninda02"`

- **Set global email**:
  
  `git config --global user.email "aninda.bhatt1992@gmail.com"`

## 3. File Operations
- **Create a new file**:
  
  `touch <filename>`

- **Remove a file**:
  
  `rm <filename>`

- **Restore a deleted file**:
  
  `git restore <filename>`

## 4. Staging and Commit
- **Check the status of the repository**:
  
  `git status`

- **Add a file to the staging area**:
  
  `git add <filename>`

- **Commit changes with a message**:
  
  `git commit -m "your commit message"`

## 5. Branching
- **Create a new branch**:
  
  `git checkout -b <branch_name>`

- **Switch between branches**:
  
  `git checkout <branch_name>`

- **List all branches**:
  
  `git branch`

## 6. Logs
- **View commit history**:
  
  `git log`

- **View concise commit history**:
  
  `git log --oneline`

## 7. Remove from Staging
- **Unstage a file (remove from index but keep in working directory)**:
  
  `git rm --cached <filename>`

## 8. Miscellaneous
- **View all files, including hidden ones**:
  
  `ls -a`

- **Clear terminal screen**:
  
  `clear`

- **View command history**:
  
  `history`

## 9. Git push using ssh and clone
- **To clone a file in local from remote**:

  `git clone https://github.com/aninda02/git-tutorial.git`

- **To make changes in local and push it to remote**:

  - Create a file in local (ex: README.md)
  - Add it to git using : git add README.md
  - Commit the changes to git: git commit -m "to add the changes"
  - Push the changes using: git push 
  - Now at this point, you would be required to enter the git username and password, and the changes would be reflected.

## 9. Git push without using username and password

**Step 1**:

  `git remote -v` - This command would give the output of push and fetch url
  `git remote set-url origin https://<token id>@github.com/aninda02/git-tutorial.git`
  `git push`

**Step 2**:

  `git remote -v` - This command would give the output of push and fetch url

   **Generate ssh keys**:
   - cd .ssh
   - ssh-keygen
   - Copy the public key (<hostname>.pub) and go to your github repository
   - Go to Settings --> SSH and GPG keys --> New SSH key --> Paste your public key

   **Git push with ssh**:

  `git remote set-url origin git@github.com:aninda02/git-tutorial.git`
  `git push`

## 10. To pull changes into local from remote

   `git pull origin main`
  
