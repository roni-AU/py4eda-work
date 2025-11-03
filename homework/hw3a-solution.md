# HW3A Solution - Git and Version Control

## Part 1: Repository Cloning
I successfully cloned the class repository from `https://github.com/olearydj/INSY6500` to
`~/insy6500/class_repo`.

### Key Commands Used
- `git clone <url> <folder_name>` - Create local copy of remote repository to a new folder
- `git log` - View commit history
- `git remote -v` - Check remote repository connections

## Part 2: Portfolio Repository Creation
I created my personal course repository with:
- Professional README.md describing the project
- Proper .gitignore to exclude unnecessary files
- Organized directory structure for homework, projects, and notes

### Understanding Git Workflow
The three-stage workflow:
1. Working Directory: Where I edit files
2. Staging Area: Where I prepare commits with `git add`
3. Repository: Where commits are permanently stored with `git commit`

## Part 3: GitHub Publishing
Successfully published repository to GitHub:
- Used `git remote add origin` to connect local repo to GitHub
- Used `git push -u origin master` to upload commits
- Proved authentication for first time use
- Refreshed the GitHub we interface and verified all files and commits are visible on GitHub

### The Remote Connection
My local repository is now connected to GitHub:
- `git remote -v` shows the remote URL
- `git push` will send my commits to GitHub
- `git pull` will get updates from GitHub (if changes are made on GitHub)

### Details
Complete this section with details from your setup:
- Repository URL: `https://github.com/roni-AU/py4eda-work`
- Output of `git remote -v`:
```bash
$ git remote -v`
origin  https://github.com/roni-AU/py4eda-work.git (fetch)
origin  https://github.com/roni-AU/py4eda-work.git (push)
```
- The output of `git log --oneline`:
```bash
$ git log --oneline`
435e586 (HEAD -> master, origin/master) Add hw3a solution document
d2fb087 Initial Commit: Add README and .gitignore
```
