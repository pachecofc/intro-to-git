# Working Directory
- Area where all of our files and directories and changes are living all the
- time.

# Staging Area
- Files and directories we explicitly want to track.
- Command: git add <file>
- Command: git add *.extension. Example: git add *.html adds all HTML files.
- git add -A. Adds all files and folders.
- git reset HEAD <file>... to unstage OR
- git rm --cached <file>...
- touch .gitignore to create a hidden file where you can type in all the files
- you want to ignore.

# Git Repository
- Where all our snapshots are stored.
- Command: git commit -m "Message in present tense"
- git log. Shows the status of our repository. Press "q" to return to command
- line.

# Git Branches
- Listing all branches: git branch

- Adding a branch allows us to make some changes to our code withou affecting
- the original code.
- git checkout -b <name of the new branch>

- Changing branches: git checkout <branch>

- Merging a branch
- Change to branch master and then git merge <branch you want to merge into
- master>
- On the GNU nano screen press Control + X

- Removing a branch
- NOT recommended
- git branch -d <branch>

# Git Checkout
Git allows us to checkout any of the commits from our log. This means we can go
back and look at the code from our earlier commits without losing any of our
current commits. This is especially useful when you're current codebase is
broken, but you have an earlier commit with working code.

The steps are as follows:

1) Make sure you're inside of your project's directory, using the cd command.
2) Once inside of the directory, use git log to view your log history.
3) You can scroll down to earlier commits by hitting enter (return)
4) Once you locate the commit you want to checkout, copy the hash key from the
commit.
    - The hash key is the alphanumeric string that comes after the word "commit"
    - The hash from above is the string of characters that begins with
    7484e645. You don't have to copy the entire sequence of characters, the
    first few will do.
5) Exit out of git log by pressing Q
6) Type git checkout 7484e645 (replace the hash with one from your selected
commit) and hit enter
7) Now you can look around inside of this commit and copy any code that you
need. If you'd like to start working from this commit, but don't want to
overwrite any of the code from the branch that you're currently on (in this
case it's master) then you can type git checkout -b <branch_name> to create a
new branch to begin working from.
8) Once you're done working from this commit, you can return to the most recent
commit on the branch of your choosing by typing git checkout <branch_name>,
in this case I typed git checkout master and it returned me to my most recent
commit on the master branch.

Note: When you checkout an earlier commit, you are now in a "detached HEAD"
state, this means that you are no longer on the commit that is being pointed to
by the HEAD. The HEAD, in git, is a pointer to the most recent commit of
whichever branch you are currently on.

# Git connection to GitHub
- Create a repository on GitHub.
- Copy the https address.
- On C9 make sure you are on your project directory.
- Type git remote add origin <https address>
- Or git remote set-url origin <https address>.
- Type git remote -v in order to view the connection.
- Type git push -u origin master.
- When asked type your username and password and hit enter.
- Check if everything worked out fine by logging in GitHub and accessing the
- project repository.