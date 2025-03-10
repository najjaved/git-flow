# lab-git-flow

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
- git stash apply