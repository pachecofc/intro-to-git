# Working Directory
- Area where all of our files and directories and changes are living all the time.

# Staging Area
- Files and directories we explicitly want to track.
- Command: git add <file>
- Command: git add *.extension. Example: git add *.html adds all HTML files.
- git add -A. Adds all files and folders.
- git reset HEAD <file>... to unstage OR
- git rm --cached <file>...
- touch .gitignore to create a hidden file where you can type in all the files you want to ignore.

# Git Repository
- Where all our snapshots are stored.
- Command: git commit -m "Message in present tense"
- git log. Shows the status of our repository. Press "q" to return to command line.

# Git Branches
- Listing all branches: git branch

- Adding a branch allows us to make some changes to our code withou affecting the original code.
- git checkout -b <name of the new branch>

- Changing branches: git checkout <branch>

- Merging a branch
- Change to branch master and then git merge <branch you want to merge into master>
- On the GNU nano screen press Control + X

- Removing a branch
- NOT recommended
- git branch -d <branch>