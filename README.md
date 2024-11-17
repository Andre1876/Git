![Git Cheat Sheet](https://www.freecodecamp.org/news/content/images/size/w2000/2021/02/git-cheat-sheet-cover.jpg)

# Git Cheat Sheet  
By Fabio Pacific  

Git is a distributed version control system that helps developers, including Andre, collaborate on projects of any scale.  
Created by Linus Torvalds in 2005, Git was designed to manage the development of the Linux kernel.

---

## What is a Distributed Version Control System?  
A distributed version control system helps you keep track of changes made to files in your project. This change history lives on your local machine and lets you revert to a previous version of your project if needed.  
Git makes collaboration easy. Each team member has a full backup of the repository locally, and using an external server like BitBucket, GitHub, or GitLab, they can safely store the repository in one place.  
By using Git, different members of the team can copy the repository locally and track changes made by everyone.

---

## Git Configuration Commands

### How to check your Git configuration:  
This command returns a list of information about your Git configuration, including your user name and email.  
### 🔶 `git config -l`

---

### How to set up your Git username:  
You can configure your username with this command.  
### 🔶 `git config --global user.name "yourusername"`

---

### How to set up your Git user email:  
This command allows you to set the email address that will be used in your commits.  
### 🔶 `git config --global user.email "youremail.com"`

---

### How to cache your login credentials in Git:  
You can store login credentials in the cache so you don’t have to type them each time.  
### 🔶 `git config --global credential.helper cache`

---

## Git Workflow Commands

### How to initialize a Git repo:  
The first step is to initialize a new Git repo locally in your project root.  
### 🔶 `git init`

---

### How to add a file to the staging area in Git:  
This command adds a file to the staging area. Replace `filename_here` with the name of the file you want to add.  
### 🔶 `git add filename_here`

---

### How to add all files to the staging area in Git:  
If you want to add all files in your project to the staging area, use the wildcard `.` to add every file.  
### 🔶 `git add .`

---

### How to add only certain files to the staging area in Git:  
To add only files that start with "fil," use the command below.  
### 🔶 `git add fil*`

---

### How to check a repository's status in Git:  
This command shows the status of the current repository, including staged, unstaged, and untracked files.  
### 🔶 `git status`

---

### How to commit changes in the editor in Git:  
This opens a text editor in the terminal where you can write a commit message.  
### 🔶 `git commit`

---

### How to commit changes with a message in Git:  
You can commit changes and include a short commit message without opening the editor.  
### 🔶 `git commit -m "your commit message here"`

---

### How to commit changes (and skip the staging area) in Git:  
You can commit tracked files and skip the staging area using the `-a` and `-m` options.  
### 🔶 `git commit -a -m "your commit message here"`

---

## Viewing Git History and Changes

### How to see your commit history in Git:  
This shows the commit history for the current repository.  
### 🔶 `git log`

---

### How to see your commit history including changes in Git:  
This command shows commit history with changes made to each file.  
### 🔶 `git log -p`

---

### How to see a specific commit in Git:  
This shows a specific commit. Replace `commit-id` with the ID of the commit you want to view.  
### 🔶 `git show commit-id`

---

### How to see log stats in Git:  
This shows statistics about changes in each commit, including the number of lines changed and the affected files.  
### 🔶 `git log --stat`

---

### How to see changes made before committing them using "diff" in Git:  
You can pass a file as a parameter to see changes on a specific file. Use `--staged` to see staged changes.  
### 🔶 `git diff`  
### 🔶 `git diff all_checks.py`  
### 🔶 `git diff --staged`

---

## Undoing Changes in Git

### How to remove tracked files from the current working tree in Git:  
This command removes files from the working tree. A commit message is required to explain the removal.  
### 🔶 `git rm filename`

---

### How to rename files in Git:  
This command renames files and stages the changes. It also expects a commit message.  
### 🔶 `git mv oldfile newfile`

---

### How to ignore files in Git:  
Create a `.gitignore` file to specify which files to ignore, then commit it.  
### 🔶 `gitignore`

---

## Branching and Merging in Git

### How to create a new branch in Git:  
This creates a new branch in your repository.  
### 🔶 `git branch branch_name`

---

### How to switch to a newly created branch in Git:  
This command switches to the branch specified.  
### 🔶 `git checkout branch_name`

---

### How to create a branch in Git and switch to it immediately:  
This creates and switches to a new branch in a single command.  
### 🔶 `git checkout -b branch_name`

---

### How to delete a branch in Git:  
After merging a branch, you can delete it using this command.  
### 🔶 `git branch -d branch_name`

---

### How to merge two branches in Git:  
This merges the current branch with another specified branch.  
### 🔶 `git merge branch_name`

---

### How to list all branches in Git:  
This lists all the branches in your repository.  
### 🔶 `git branch`

---

### How to list remote branches in Git:  
This lists all the remote branches.  
### 🔶 `git branch -r`

---

### How to check out a remote branch in Git:  
This command checks out a remote branch for local use.  
### 🔶 `git checkout --track origin/branch_name`

---

### How to rebase a branch in Git:  
This command helps you reapply your changes on top of another branch.  
### 🔶 `git rebase branch_name`

---

## Remote Repositories in Git

### How to add a remote repository in Git:  
This command adds a remote repository to your local Git repository.  
### 🔶 `git remote add origin https://repo_here`

---

### How to push changes to a remote repo in Git:  
This pushes your changes to the remote repository.  
### 🔶 `git push`

---

### How to push a specific branch to a remote repo in Git:  
This command pushes a specific branch to the remote repository.  
### 🔶 `git push origin branch_name`

---

### How to pull changes from a remote repo in Git:  
If other team members have made changes, you can retrieve their latest updates using this command.  
### 🔶 `git pull`

---

### How to fetch changes from a remote repo in Git:  
This retrieves the latest changes without merging them.  
### 🔶 `git fetch`

---

### How to clone a repository in Git:  
This command creates a local copy of a remote repository.  
### 🔶 `git clone https://repo_here`

---

### How to remove a remote repository from Git:  
This command removes a remote repository from your local configuration.  
### 🔶 `git remote remove origin`

---

## Advanced Git Commands

### How to stash changes in Git:  
This saves your changes temporarily so you can work on something else.  
### 🔶 `git stash`

---

### How to list all stashes in Git:  
This command shows all the saved stashes.  
### 🔶 `git stash list`

---

### How to apply a stash in Git:  
This restores the changes you stashed earlier.  
### 🔶 `git stash apply`

---

### How to apply a specific stash in Git:  
You can apply a specific stash by referring to its ID.  
### 🔶 `git stash apply stash@{stash_id}`

---

### How to drop a stash in Git:  
This removes a stash from the list.  
### 🔶 `git stash drop stash@{stash_id}`

---

### How to create a tag in Git:  
Tags are useful for marking specific points in history.  
### 🔶 `git tag tag_name`

---

### How to list tags in Git:  
This command lists all tags in the repository.  
### 🔶 `git tag`

---

### How to push tags to a remote repo in Git:  
This pushes tags to the remote repository.  
### 🔶 `git push origin tag_name`

---

### How to delete a local tag in Git:  
You can delete a tag from your local repository.  
### 🔶 `git tag -d tag_name`

---

### How to revert a commit in Git:  
This command allows you to undo a commit by creating a new commit that reverts the changes made.  
🔶 `git revert commit_id`

---

### How to check the differences between two commits in Git:  
This command shows the differences between two commits. Replace `commit_id1` and `commit_id2` with actual commit IDs.  
🔶 `git diff commit_id1 commit_id2`

---

### How to pull changes from a remote repo in Git:  
If other team members have made changes, you can retrieve their latest updates using this command.  
🔶 `git pull`

## Conclusion  
These Git commands can significantly boost your productivity. You don't need to memorize all of them—just refer to this cheat sheet whenever needed. Fork this repo and print it for future reference.  

A big thanks to Fabio, a full-stack web developer and IT automation professional, for creating this helpful content. You can find more useful material on his YouTube channel: [Fabio's YouTube Channel](https://www.youtube.com/channel/UCTuFYi0pTsR9tOaO4qjV_pQ)  

---
