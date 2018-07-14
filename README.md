# Commands Synopsis

## bash commands

touch filename === to create a file
ls === list files in a folder
rm -rf foldername === to recursively remove a folder

## PS command

code === to create file
code .gitignore === to create a .gitignore file
ls === list files
ls -Force === lists files and folders including hidden

## git commands

git help {git command} provide helps for a specific commang
git help {git command} --oneline === provide help info on one line
git config --global -e
git init . === initialize the current folder === the period denotes the current folder.
git status === to get current status of project

git log === show listing of commits in repository
git log --oneline --graph --decorate --all ===== shows a conveniently modifed history of git
git config --global alias.hist "log --oneline --graph --decorate --all"  === creates an alias for the above line
git hist === Now we can use this command instead of typing all the flags

git show === shows most recent commit and diffs.  In PS have to use q to quit
git ls-files === show what files git is tracking

git add filename === to add file to git tracking systme
git add . === to add untracked files to git tracking system
git add -u === picks up changes to files that have been updated but not those added  === must be followed by commit
git add -A === adds all types of changes to staging === e.g. addition and deletion   === must be followed by commit

git reset HEAD filename  === unstages a file
git checkout === filename === undos changes
git commit -m
git commit
git commit -am "Add Commit Message here"  ===Express Commit === add modified files to staging and commits them

git vm oldfilename newfilename === renames a file  === must be followed by a commit
git rm filename === removes filename from project  === must be followed by a commit

### Branching

git checkout nameOfBranch === switches to branch named in nameOfBranch
git branch === displays all branches
git checkout -b updates === creates a new branch call 'updates' with HEAD pointing to it.
