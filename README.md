# Git-Cheatsheet
🐱A Cheatsheet for Git 

## Fundamentals
| Term | Description |
| ----------- | ----------- |
| Working Tree | Directory where modifications are made |
| HEAD | Symbolic Reference to the most recent commit |
| Index(Staging Area) | This is where commits will be prepared |
| Repository | Different states of files will be tracked inside the Repository |

![Cheat: Terminal Cheatsheet](https://github.com/SebastianBoldt/Git-Cheatsheet/blob/e12a338944a5ca89aae5298119f7c96a81f52e8f/Images/index.png?raw=true)

## Commands 

| Command | Description |
| ----------- | ----------- |
| git config --global user.name "Max Mustermann" | Configure global username |
| git config --global user.email "m.mustermann@example.com" | Configure global email adress |
| git config -l | show all configurations for current repo |
| git config alias.\<alias-name\> \<alias\> | create a alias |
| git config --global alias.\<alias-name\> \`config --global\` | create alias with parameters |
| git config color.ui auto | set color options to automatic mode |
| git init example  | initalise git repository |
| git status | show current repository status |
| git add file | add file to the staging area|
| git add . | add all changes made to the staging area |
| git add --p | git will ask you which files you want to add to the staging area |
| git commit -m "First Commit" | Commit changes to current branch |
| git commit --amend | Repair commit (SHA-1 Hash will change) |
| git show | show last commit message etc. |
| git show HEAD | show newest commit |
| git show master | show latest commit of branch master |
| git show 77cc0045 | show commit with hash 77cc0045 |
| git log | show all commits |
| git diff | show difference between working tree, staging area and repo |
| git diff --staging | show difference between staging area and repo |
| git reset A.txt | Removes file from staging area |
| git reset HEAD | reset the staging area  |
| git reset --p | git will ask you which files you want to remove from the staging area |

## Files

| Filename | Description |
| ----------- | ----------- |
| ~/.gitconfig  | Configuration for all repositories - global |
| /etc/gitconfig | system wide configurations |

... to be continued.

## Update Tags

git tag -l | xargs git tag -d

git fetch --tags
