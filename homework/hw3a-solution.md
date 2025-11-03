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
- Repository URL: <https://github.com/roni-AU/py4eda-work>
- Output of `git remote -v`:
```bash
$ git remote -v
origin  https://github.com/roni-AU/py4eda-work.git (fetch)
origin  https://github.com/roni-AU/py4eda-work.git (push)
```
- The output of `git log --oneline`:
```bash
$ git log --oneline
435e586 (HEAD -> master, origin/master) Add hw3a solution document
d2fb087 Initial Commit: Add README and .gitignore
```

## Questions

### Reflections

#### Question 1: Git Workflow Benefits

a) Before doing this assignment, I usually managed different versions of my assignments, writings and code by saving extra copies with filenames like "v1.1", "v1.3", or sometimes filename followed by the datae of modification. This method was sometimes confusing and made it hard to know what changed or why. Git provides following benefits over my earlier practice:
- Automatic change tracking with timestamps and comments[e.g.: "Updated assignment documentation"].
- Easy rollback to previous versions as needed.
- Collaboration features that avoid overwriting by making the repository read only.

b) In a past group project for STAT 7000, each of our 4 team members wrote some specific parts of the code. After fist compilations, our results were not satisfactory and we decided to filter the dataset and reanalyze. Then we ended up ended up overwriting each other’s files. Using Git’s commit history would have helped to identify who did what and recover files and track changes, making teamwork much smoother.

#### Question 2: Repository Organization

a) Keeping the class repository and my own repository separate is important because each serves a different purpose. Putting everything into one repository would make it hard to tell which files belong to me and which are reference materials, and could lead to accidental changes in the original reference materials.

b) For future coursework, I’d keep separate repositories for group projects and individual assignments. Reference materials should be put into their own read-only repository, so they’re not mixed up with my own work or team files.

#### Question 3: Commit Messages and History

a) The message “Add hw3a solution documenting Git workflow and repository structure” is far more useful than “update.” It clearly describes the purpose of commit, so I could easily find this solution or explain changes to someone else. General messages make it hard to know what was actually changed.

b) In a multi-week data analysis project, I’d make a commit after achieving a defined milestone, like cleaning data, finishing a function, or generating a graph. Each commit should represent a specific “unit of work” that stands on its own for clarity when reviewing history.


### Graduate Questions

#### Question 1: The Three-Stage Model

a) Committing the README.md and .gitignore files together first was valuable because these files set up the structure and ignored files for the project. Committing hw3a-solution.md separately later helped keep changes organized by logical steps. If I had committed everything at once, the commit history would be less clear, making it harder to understand what each commit represents or to revert specific changes later.

b) I would commit changes like loading data and fixing typos immediately since they are complete and meaningful units of work. For the half-finished analysis function, I would wait to commit until it is more complete to avoid saving unfinished or broken code. Staging allows me to select only the ready changes, so I can separately commit polished parts and keep work-in-progress out of the history.

c) `git status` shows which files have changed and which are staged. I use it before staging to see what needs to be added, and after staging to confirm precisely what will be committed. It helps make informed decisions about grouping related changes together to create a clean commit history.

#### Question 2: Local vs. Remote Repositories

a) Git being a distributed system means every developer has a full copy of the repository history locally, unlike Google Drive or Dropbox that just sync files without version history or branching. This allows working offline and makes operations like commits and history browsing fast and independent of network.

b) Working locally without internet is valuable because I can continue coding, committing, and reviewing history anywhere. Later, pushing changes syncs them with the remote GitHub repository. This enables flexible workflows like offline work and asynchronous collaboration.

c) `git clone` copies a remote repository locally. `git pull` fetches and merges remote changes into my local repository. `git push` uploads my committed changes to the remote repository. I can pull from `class_repo` because it’s read-only for me (no push permission), but I can push to `my_repo` because it’s my own remote repository where I have write access.

#### Question 3: Professional Portfolio

a) When deciding what to commit, I will consider balancing showing my workflow including mistakes and iterations. I will commit work that reflects my skills and growth, keeping drafts separate from polished results. I will avoid unnecessary or sensitive files and use clear commit messages to show progress while maintaining a professional presentation.

b) A portfolio README should highlight who I am, the purpose of the repository, and an overview of the work done with clear instructions to understand it. This differs from an open-source README, which focuses more on how to install, use, and contribute to the project.

c) Building a public portfolio during coursework is valuable because it motivates good version control habits, documents ongoing learning, and provides evidence of skills to employers in advance. Developing consistent commit messaging, clear docmentation, and regular update make the portfolio more impressive and useful later.
