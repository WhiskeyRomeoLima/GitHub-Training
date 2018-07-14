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

git checkout nameOfBranch === switches to branch called nameOfBranch
git branch === displays all branches
git checkout -b updates === creates a new branch call 'updates' with HEAD pointing to it.
git branch -d nameOfBranch === deletes branch called nameOfBranch

#### Example of branching and merging

PS F:\visual studio 2017\Training\GitHub Ultimate\projects\demo> git branch
* master
PS F:\visual studio 2017\Training\GitHub Ultimate\projects\demo> git checkout -b updates <!-- created new branch -->
Switched to a new branch 'updates'
M       README.md
PS F:\visual studio 2017\Training\GitHub Ultimate\projects\demo> git add . <!-- added changes to staging -->
PS F:\visual studio 2017\Training\GitHub Ultimate\projects\demo> git commit -m 'adding updates to Readme.md in the updates branch'
[updates 9bd513d] adding updates to Readme.md in the updates branch
 1 file changed, 4 insertions(+), 1 deletion(-)
 <!-- now do git hist to see head points to updates branch -->
PS F:\visual studio 2017\Training\GitHub Ultimate\projects\demo> git hist
* 9bd513d (HEAD -> updates) adding updates to Readme.md in the updates branch
* cb449b5 (master) updates to README.md in the updates branch
* 28764ca updates to README.md in the updates branch
* f790fa9 updates to README.md in the updates branch
* ccc7018 changes to README.md
* 78a8a09 updating Readme
* 27bd010 updating Readme
* cc94713 this is a commit