# Git-Cheatsheet
A Cheatsheet for Git 

## Fundamentals
| Term | Description |
| ----------- | ----------- |
| Working Tree | Directory where modifications are made |
| HEAD | Symbolic Reference to the most current checked out commit - can be detached so it points to another commit |
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
| git reset HEAD~3 | resets current branch to HEAD - 3 Commit |
| git revert COMMIT_HASH | reverts to old state by creating a new commit |
| git branch BRANCHNAME | creates a new branch named BRANCHNAME |
| git checkout BRANCHNAME | moving to a branch with the name BRANCHNAME |
| git checkout COMMIT_HASH | detach HEAD and move it to the commit with the hash COMMIT_HASH |
| git checkout main^ | moves head to previous commit |
| git checkout main^2 | if current commit is merge commit it checks out the second one | 
| git rebase BRANCHNAME | rebasing the current branch to BRANCHNAME |
| git rebase -i HEAD~4 | start an interactive rebase to change the last 4 commits |
| git checkout HEAD^ | moves HEAD one commit back in time |
| git checkout HEAD~ | moves HEAD to previous commit |
| git branch -f main HEAD~3 | moves branch to HEAD - 3 Commit |
| git cherry-pick HASH1 HASH2 ... | pick all the commits and apply them to the current branch |
| git tag v1 COMMIT_HASH | append tag v1 to commit with hash COMMIT_HASH |
| git describe TAGNAME | shows you how many commit are between you and the tag with name TAGNAME (v2_1_gC4) -> (NEXT-TAG_NUMBEROFCOMMITS_COMMITHASH) |
| git checkout -b not_main origin/main | creates a local branch not_main that tracks the remote branch main |
| git branch -u origin/main foo | let foo track remote branch origin/main so push and pull operate on it |
| git fetch | moves changes to local remote tracking branch |
| git pull | fetches all changes and merges them in corresponding local branch |
| get pull --rebase | fetches all changes and rebases them before on the current branch commits |
| git push origin main | pushes all changes from main to origin main |
| git push origin SOURCE:DESTINATION | pushes all changes from local SOURCE to remote DESTINATION on origin |
| git push origin main^:foo | pushes all changes from local main - 1 commit to remote foo on origin |

## Files

| Filename | Description |
| ----------- | ----------- |
| ~/.gitconfig  | Configuration for all repositories - global |
| /etc/gitconfig | system wide configurations |

... to be continued.

## Update Tags

git tag -l | xargs git tag -d

git fetch --tags
