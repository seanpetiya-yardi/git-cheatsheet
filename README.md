# git-cheatsheet
cheatsheet for git commands. note `dev` is the `main` branch.

# branches
:star: **create** new branch: `git checkout -b "feature/new-branch"`  
:scissors: **prune** old branches: `git fetch --prune`  
🥇 **pull origin**: `git pull origin dev`  
🍥 set the **upstream** branch: `git branch --set-upstream-to=origin/dev dev`

# commits
🐈‍⬛ empty commit with **message**: `git commit --allow-empty -m "my commit message"`  
:bug: **amend** commit message: `git commit --amend`

# errors
🌊fix **upstream branch of your current branch does not match the name of your current branch**: `git branch --unset-upstream`  
⛵fix **there is no tracking information for the current branch**: `git pull origin dev` AND/OR `git branch --set-upstream-to=origin/dev dev`

