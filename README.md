# lab-git-flow

**Git Cmds Cheatsheet**
- git --version
- git config --global user.name "Your Name"
- git config --global user.email "youremail@example.com"
- git config --list

******************************************
- echo "# lab-git-flow" >> README.md
- git init
- git add README.md
- git commit -m "first commit"
- git branch -M main/trunk
- git remote add origin <here remote URL>
- git push -u origin main

********************************************
- git branch
- git branch feature-branch
- git checkout feature-branch / git switch feature-branch
- git switch - (switch back to previously checked out branch)
- git merge feature-branch
- git push origin main

********************************************
useful when switching branches without committing unfinished work
- git stash
- git stash list
- git stash apply (Re-applies the changes from the most recent stash to your working directory)
- git stash apply stash@{1} (to apply a specific stash)

********************************************
- git log
- git show [commit-hash]

***Git reset to undo changes:***
- git reset example.txt (remove a file from the staging area)
- git reset --hard (resets working directory and staging area to match the most recent commit. This means any changes, whether staged or not, will be lost)
- git reset --hard HEAD~1 (HEAD~1 referes to move one commit backwards current commit (HEAD))
- git clean -n (remove untracked files from your working directory)
- git clean -f

*** Editing commit msgs ***
- git commit --amend -m "Your new commit message" (edit most recent commit)
- git rebase -i HEAD~n  # Replace 'n' with the number of commits you want to go back
(In the editor that opens, type i, change 'pick' to 'reword' for the desired commit, press escape, press :wq and enter, save, and follow the prompts.)

**********************************************
## Tagging:
Tagging helps in versioning (mark specific points in your project's history as important). Tags are like labels that you can attach to a specific commit, making it easy to identify significant versions of your project, such as releases.
- git tag -a v1.0 -m "Version 1.0 release"
- git tag (see a list of all tags in your repository)
- git show v1.0




