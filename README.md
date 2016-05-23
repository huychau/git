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
      - `git branch -D branch-name-1 branch-name-2 ...`
      - Branch name start with `origin/feature/`:
      `git branch | grep 'origin\/feature\/*' | xargs git branch -d`
    - Remote:
      `git push origin :<branch name>`
