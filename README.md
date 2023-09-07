# Cheat-Sheet for quick use of Git & GitHub 
![install-git-for-multiple-users-removebg-preview (1)](https://user-images.githubusercontent.com/46279617/147650960-d4116f9f-0822-44a7-9c85-edb80da3ab04.png)

- make sure you have git installed or [download-here](https://git-scm.com/downloads)
- Get started with Git Bash

## How Git works
![#Files](https://miro.medium.com/max/700/1*e1tZOAcVCtfXUWW7VqHDzA.png)

### First create a directory
- Git will create a folder in C disk C:/Users/user/dirname 
```
mkdir directoryname
```
### Initialise the directory
- Git will initialise the directory in C disk C:/Users/user/dirname/.git/
- initializes a new Git repository and begins tracking an existing directory. It adds a hidden subfolder within the existing directory that houses the internal data structure required for version control
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
git diff filename
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
## :warning: Create an repositories and have its https link copied before moving ahead like the following one :warning:
![repo link example](https://user-images.githubusercontent.com/46279617/162811236-c67d8f8d-c223-4d04-918c-1b14fdba4008.jpg)
### push an existing repository from the command line
```
echo "# gittest" >> README.md
```
```
git push -u origin main
```
```
git init
```
```
git add README.md
```
```
git commit -m "first commit"
```
```
git branch -M main
```
```
git remote add origin https://github.com/kiranbakale/gittest.git
```
### Configuring our local repository to move files remote repository  
- If we type in command it will be connected to remote repository

```
git remote add repo or aliasname repo url
```
### Selecting a branch
```
git branch -M main
```
### Finally pushing our docs from local to an remote repository
- Git will push our docs in local repo to master branch in remote repo 
```
git push -u origin main
```
### Updating Local docs with docs in remote repository
- Git helps developers use this command if at all made commits to a branch on a remote-repo, and they would like to reflect those changes in their local environment
```
git pull aliasname branch
```
## Branching

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
## Cloning
Git clone is a command for downloading existing source code from a remote repository (like Github, for example). Git clone basically makes an identical copy of the latest version of a project in a repository and saves it to your computer.
```
git clone -b <Branch name><Repository URL>  

```


### Command for unstaging the file which is added in the staging environment
```
git restore --staged filename
```
- History of the commits
```
git logs
```
- To jumping to specific commit and deleting the older 


```
git reset commit-hash-id
```

- HEAD is a pointer that will point to current working branch
and also say in which branch, the latest commits will be pushed.



unstaging a commit that is already being pushed to remote repo

```
git reset below-commit-log-id
```
```
git add .
```
```
git stash
```
```
git push origin kk -f
```

fetching commits from upstream repo and keeping our repo insync with upstream repo
```
git fetch --all --prune

git reset --hard upstream

git push origin main

squashing the commits

git rebase -i commit-hash

```
### Pointers

- upstream is the parent repo
- Any new thing you are working on create a new branch in local start
working from there
- 1 pull req = 1 branch
- If you want to push newly created remote repo, then command
```
git push origin branchname
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

