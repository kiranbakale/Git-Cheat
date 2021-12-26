# Cheat-Sheet for quick use of Git & GitHub 

![#Files](https://o.remove.bg/downloads/c34af629-2b18-4b31-ae94-9e177da26655/install-git-for-multiple-users-removebg-preview.png) 
<!-- <img src="https://github.com/favicon.ico" align="center" height="48" width="48" left="60" top="10"></a> -->

<!-- ![test](https://github.com/favicon.ico) -->
<!-- ![image](https://github.com/favicon.ico) -->
- make sure you have git installed or [download-here](https://git-scm.com/downloads)
- Get started with Git Bash
### First create a directory
- Git will create a directory in C disk C:/Users/user/dirname 
```
mkdir directoryname
```
### Initialise the directory
- Git will initialise the directory in C disk C:/Users/user/dirname/.git/
```
git init![68747470733a2f2f6f2e72656d6f76652e62672f646f776e6c6f6164732f63333461663632392d326231382d346233312d616539342d3965313737646132363635352f696e7374616c6c2d6769742d666f722d6d756c7469706c652d75736572732d72656d6f766562672d707265766965772e706e67](https://user-images.githubusercontent.com/46279617/147405074-5725f881-9114-4c7c-979e-ae4f36d919b7.png)

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
