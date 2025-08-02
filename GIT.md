# Git Commands Cheat Sheet 🧠

Quick reference for Git commands, formatted for developers. All commands are in code blocks for clarity.

*Updated: August 1, 2025*

```bash
# Setup
git config --global user.name "Your Name"  # Set username
git config --global user.email "your@email.com"  # Set email
git config --list  # View config

# Repository
git init  # Initialize new repo
git clone <repo-url>  # Clone a repo
git status  # Check working directory status
git add <file>  # Stage file
git add .  # Stage all changes
git commit -m "message"  # Commit changes
git log  # View commit history
git show <commit>  # Show commit details
git diff  # View unstaged changes
git diff --staged  # View staged changes

# Branching
git branch  # List branches
git branch <name>  # Create branch
git checkout <branch>  # Switch branches
git checkout -b <branch>  # Create and switch
git merge <branch>  # Merge into current branch
git rebase <branch>  # Reapply commits
git branch -d <branch>  # Delete branch

# Remote
git remote -v  # List remotes
git remote add origin <url>  # Add remote
git push -u origin main  # Push and set upstream
git push origin main  # Push to remote
git pull  # Pull from remote
git fetch  # Fetch without merging

# Undo
git reset <file>  # Unstage file
git reset --soft HEAD~1  # Undo commit, keep staged
git reset --hard  # Undo all changes (careful!)
git checkout -- <file>  # Discard local changes
git revert <commit>  # Undo with new commit

# Tags
git tag  # List tags
git tag <v1.0>  # Create tag
git push origin <tag>  # Push tag

# Collaboration
git pull origin main  # Pull latest
git push origin <branch>  # Push branch
git stash  # Save changes
git stash pop  # Restore stashed changes
