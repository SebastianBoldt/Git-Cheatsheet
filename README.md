# Git-Cheatsheet
🐱A Cheatsheet for Git 

##Commands 

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
| git add file | add file to git tracked files |
| git commit -m "First Commit" | Commit changes to current branch |
| git show | show last commit message etc. |
| git show HEAD | show newest commit |
| git show master | show latest commit of branch master |
| git show 77cc0045 | show commit with hash 77cc0045 |
| git log | show all commits |

##Files

| Filename | Description |
| ----------- | ----------- |
| ~/.gitconfig  | Configuration for all repositories - global |
| /etc/gitconfig | system wide configurations |




