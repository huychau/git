# Use Git basic
1. Git add
  - Add files/folders:
    `git add file/folder name`
  - Add all files change:
    `git add .`
  - Reset files/folders
    `git reset file/folder`
  - Reset all files change
    `git reset .`
  
1. Git commit
  - Commit: 
    `git commit -m "[Isuse ID] Message"`
  - Edit commit:
    `git commit --amend -m "[Isuse ID] Message"`
  - Reset commit:
    - Last commit:
      `git reset --soft HEAD~`
    - Commit id:
      `git reset --hard <COMMIT -ID>`
1. Git push
  `git push origin <branch name>`
1. Branch
  - Delete:
    - Local:
      `git branch -D <branch name>`
    - Multiple branches: 
      - `git branch -D branch-name-1 branch-name-2 ...
      - Branch name start with `origin/feature/`:
      `git branch | grep 'origin\/feature\/*' | xargs git branch -d`
    - Remote:
      `git push origin :<branch name>`
      
## Git flow simple step by ste
1. Install
```
sudo apt-get install git-flow
```
1. Config
```
cd your-folder
git flow init
```
 _Note: Enter all if you don't need modifier_

1. Branch
 - Create branch
```
git flow feature branch-name (create base on develop)
git flow hotfix branch-name (create base on master)
```
 - Finish up a feature (branch)
  + Merges MYFEATURE into 'develop'
  + Removes the feature branch
  + Switches back to 'develop' branch
```
git flow feature finish branch-name
```
 _Note: See about `Branch` for more details_
