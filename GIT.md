
# 🧠 Git Commands Cheat Sheet



## 🛠️ Setup

git config --global user.name "Your Name" : Set your Git username

git config --global user.email "your@email.com" : Set your Git email

git config --list : View current Git config



## 📁 Repository

git init : Initialize a new Git repo

git clone <repo-url> : Clone a repo

git status : Show status of working directory

git add <file>  /  git add . : Stage changes

git commit -m "message" : Commit staged changes

git log : Show commit history

git show <commit> : Show details of a commit

git diff : Show unstaged changes

git diff --staged : Show staged changes



## 🌿 Branching

git branch : List branches

git branch <name> : Create a branch

git checkout <branch> : Switch branches

git checkout -b <branch> : Create + switch

git merge <branch> : Merge a branch into current

git rebase <branch> : Reapply commits on another base

git branch -d <branch> : Delete branch



## 🔄 Remote

git remote -v : List remotes

git remote add origin <url> : Add remote

git push -u origin main : Push and set upstream (track remote branch)

git push origin main : Push to remote (without setting upstream)

git pull : Pull from remote

git fetch : Download but don’t merge



## 🧪 Undo

git reset <file> : Unstage

git reset --soft HEAD~1 : Undo commit (keep staged)

git reset --hard : Undo all changes (careful!)

git checkout -- <file> : Discard local changes

git revert <commit> : Undo by creating new commit



## 📦 Tags

git tag : List tags

git tag <v1.0> : Create tag

git push origin <tag> : Push tag



## 👥 Collaboration

git pull origin main : Pull latest changes

git push origin <branch> : Push branch

git stash : Save local changes

git stash pop : Restore stashed changes



## 🧠 Concepts

•    Working Directory: Your files

•    Staging Area: Prepares files to be committed

•    Commit: A snapshot of the project

•    Branch: A series of commits

•    Merge: Combine two branches

•    Rebase: Reapply commits on top of another branch



## ❓  git push -u origin main  vs  git push origin main 

git push -u origin main : Push and set the *upstream* — after this, you can just run  git push  or  git pull  without arguments.

git push origin main : Push to remote, but *does not track* the branch — you’ll always need to specify branch next time.
