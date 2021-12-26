# Cheat-Sheet for quick use of git & GitHub

### First create a directory
- Git will create a directory in C disk C:/Users/user/dirname 
```
mkdir directoryname
```
### Initialise the directory
- Git will initialise the directory in C disk C:/Users/user/dirname/.git/
```
git init
```
### Moving our files to staging area
- Typing following command files will be moved to staging area
```
git add filename
```
### Have a look at the changes
- We will know changes in form of description effected after each save of the specific document
```
git diff
```
- We will get to know various changes that we made to our whole project
```
git status
```
### Saving changes to file (failing which we cant push our files to repo)
- Entering below command will save the doc files will fall into local repository
```
git commit -a -m 'the message we want here to be displayed here'
```
## Create an repositories and have its https link copied before moving ahead
### Configuring our local repository to move files remote repository  
- If we type in command it will be connected to remote repository

```
git remote add repo or aliasname repo url
```
## Finally pushing our docs from local to an remote repository
- Git will push our docs in local repo to master branch in remote repo 
```
git push repooraliasname master
```

# Branching

- Git will create a different branch 
```
git branch branchname
```
- Helps to switch to a different branch 
```
git checkout branchname
```
## Merging
- Git will integrate/merge two different branches 
```
git merge branchname
```
## For Merge-conflicts
- A tool pops up and highlights problems causing the conflicts
```
git mergetool
```
For exiting the tool 
- After successful changes type in following command to exit
```
:wq
```
