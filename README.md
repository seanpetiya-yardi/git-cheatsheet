# git-cheatsheet
cheatsheet for git commands. note `dev` is the `main` branch.

# branches
:star: **create** new branch: `git checkout -b "feature/new-branch"`  
:scissors: **prune** old branches: `git fetch --prune`  
🥇 **pull origin**: `git pull origin dev`  
📝 **rename** branch: `git branch -m "feature/new-branch-name"`  
🍥 set the **upstream** branch: `git branch --set-upstream-to=origin/dev dev`  
🤖 **update** remote branches: `git remote update origin --prune`

# commits
🐈‍⬛ empty commit with **message**: `git commit --allow-empty -m "my commit message"`  
:bug: **amend** commit message: `git commit --amend`  
🌭**reset** local commits w/o undoing changes: `git reset --soft HEAD~1`
🌵**revert** remote commit: `git revert` + commit hash

# errors
🌊fix **upstream branch of your current branch does not match the name of your current branch**: `git branch --unset-upstream`  
⛵fix **there is no tracking information for the current branch**: `git pull origin dev` AND/OR `git branch --set-upstream-to=origin/dev dev`  
:hammer: fix **you have not concluded your merge (MERGE_HEAD exists)**: `git reset --abort`  

# forks
🐶**sync** fork; _fetch_ upstream repo: `git fetch upstream`   
🍴**sync** fork; _merge_ upstream repo: `git merge upstream/main`

