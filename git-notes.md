# Git Notes
## 2/29/2024
---
# Intro

- **git** - FOSS version control system
    - **version control** - mgmt of changes to docs, programs, configs, and other info  
## basic git commands 
- `git` - base command 
- `clone` -  downloads remote repo to local machine
- `add` - track files and changes in git 
- `commit` - save files and change in git 
- `push` - upload git commits to remote repo
- `pull` - download change from remote repo to local
---
# basic procedures 
## starting w/ remote repo 
- `git clone [REMOTE REPO URL]` - clones the repo from a remote repo
    - by default, files are inside folder with repo's name
    - `git clone [remote URL] .` to clone only files to current directory 
        - folder must be empty (can't even have `.git` file)
- `git status` - shows all files that have been modified by not yet committed
    - also shows untracked files 
- if files untracked, use `git add` to track files 
    - can use `git add .` to auto track any new files within repo 
    - can also specify specific files with `git add [NAME] [NAME 2]
- `git commit -m "MESSAGE"` - saves changes with a commit
    - `-m` - message; is required for all commits 
    - can add second `-m` after first msg to insert description 
    - `commit` saves changes to local repo only 
- `git push` - saves changes to remote repo (e.g. Github, Gitlab)
    - `git push origin main` - pushes to main branch of remote repo
        - `main` can be named other things as well; may be `master` by default for some 
    - `origin` - location of remote git repo ???
## 