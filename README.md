# Working Directory
- Area where all of our files and directories and changes are living all the time.

# Staging Area
- Files and directories we explicitly want to track.
- Command: git add <file>
- Command: git add *.extension. Example: git add *.html adds all HTML files.
- git add -A. Adds all files and folders.
- git reset HEAD <file>... to unstage.
- touch .gitignore to create a hidden file where you can type in all the files you want to ignore.

# Git Repository
- Where all our snapshots are stored.
- Command: git commit -m "Message in present tense"
- git log. Shows the status of our repository.