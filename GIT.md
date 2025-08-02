🧠 Git Commands Cheat Sheet

A quick reference for essential Git commands and concepts to streamline your workflow.

Created: August 1, 2025



🛠️ Setup





Set your Git username: git config --global user.name "Your Name"



Set your Git email: git config --global user.email "your@email.com"



View current Git config: git config --list

📁 Repository





Initialize a new Git repo: git init



Clone a repo: git clone <repo-url>



Show status of working directory: git status



Stage changes: git add <file> or git add .



Commit staged changes: git commit -m "message"



Show commit history: git log



Show details of a commit: git show <commit>



Show unstaged changes: git diff



Show staged changes: git diff --staged

🌿 Branching





List branches: git branch



Create a branch: git branch <name>



Switch branches: git checkout <branch>



Create + switch: git checkout -b <branch>



Merge a branch into current: git merge <branch>



Reapply commits on another base: git rebase <branch>



Delete branch: git branch -d <branch>

🔄 Remote





List remotes: git remote -v



Add remote: git remote add origin <url>



Push and set upstream: git push -u origin main



Push to remote (without setting upstream): git push origin main



Pull from remote: git pull



Download but don’t merge: git fetch

🧪 Undo





Unstage: git reset <file>



Undo commit (keep staged): git reset --soft HEAD~1



Undo all changes (careful!): git reset --hard



Discard local changes: git checkout -- <file>



Undo by creating new commit: git revert <commit>

📦 Tags





List tags: git tag



Create tag: git tag <v1.0>



Push tag: git push origin <tag>

👥 Collaboration





Pull latest changes: git pull origin main



Push branch: git push origin <branch>



Save local changes: git stash



Restore stashed changes: git stash pop

🧠 Concepts





Working Directory: Your files



Staging Area: Prepares files to be committed



Commit: A snapshot of the project



Branch: A series of commits



Merge: Combine two branches



Rebase: Reapply commits on top of another branch

❓ git push -u origin main vs git push origin main





git push -u origin main: Pushes and sets the upstream — after this, you can just run git push or git pull without arguments.



git push origin main: Pushes to remote but does not track the branch — you’ll need to specify the branch next time.



Note: Use this cheat sheet as a quick reference for Git commands during development. Happy coding! 🚀
Last updated: August 1, 2025
