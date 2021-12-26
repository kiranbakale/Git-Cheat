# Cheat-Sheet for quick use of git & GitHub

### First create a directory
--it will create a directory in C disk C:/Users/user/dirname 
```
mkdir directoryname
```
### Initialise the directory
it will initialise the directory in C disk C:/Users/user/dirname/.git/
```
git init
```
### Moving our files to staging area
if we type in 
--it will fall in staging area
```
git add filename
```
### Have a look at the changes
if we type in 
--We will know changes in form of description effected after each save of the specific document
```
git diff
```
--We will get to know various changes that we made to our whole project
```
git status
```
### Saving changes to file (failing which we cant push our files to repo)
if we type in 
--it will fall into local repository
```
git commit -a -m 'the message we want here to be displayed here'
```
## Create an repositories and have its https link copied before moving ahead
### Configuring our local repository to move files remote repository  
if we type in 
--it will be connected to remote repository

```
git remote add repo or aliasname repo url
```
if we type in 
--it will push our docs in local repo to master branch in remote repo 
```
git push repooraliasname master
```
if we type in 
--it will create a different branch 
```
git branch branchname
```
--it switch to a different branch 
```
git checkout branchname
```
if we type in 
--it will integrate/merge two different branches 
```
git merge branchname
```
For Merge-conflicts
--a tool pops up and highlights problems causing the conflicts
```
git mergetool
```
For exiting the tool 
-- After successful changes type in following to exit
:wq
