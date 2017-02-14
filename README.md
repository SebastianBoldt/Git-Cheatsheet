# Git-Cheatsheet
🐱A Cheatsheet for Git 

## Fundamentals
| Term | Description |
| ----------- | ----------- |
| Working Tree | Directory where modifications are made |
| HEAD | Symbolic Reference to the most recent commit |
| Index | This is where commits will be prepared |
| Repository | Different states of files will be tracked inside the Repository |

![Cheat: Terminal Cheatsheet](https://github.com/SebastianBoldt/Git-Cheatsheet/blob/master/Images/index.png?raw=true)

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
| git add file | add file to the index|
| git add . | add all changes made to the index |
| git add --p | git will ask you which files you want to add to the index |
| git commit -m "First Commit" | Commit changes to current branch |
| git commit --amend | Repair commit (SHA-1 Hash will change) |
| git show | show last commit message etc. |
| git show HEAD | show newest commit |
| git show master | show latest commit of branch master |
| git show 77cc0045 | show commit with hash 77cc0045 |
| git log | show all commits |
| git diff | show difference between working tree, index and repo |
| git diff --staging | show difference between index and repo |
| git reset HEAD | reset the index  |
| git reset --p | git will ask you which files you want to remove from the index |

## Files

| Filename | Description |
| ----------- | ----------- |
| ~/.gitconfig  | Configuration for all repositories - global |
| /etc/gitconfig | system wide configurations |

... to be continued.


