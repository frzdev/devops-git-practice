GIT CHEAT SHEET
🔹 1. Setup & Config
git --version
git config --global user.name "Your Name"
git config --global user.email "you@email.com"
git config --list
🔹 2. Create / Clone Repository
git init
git clone <repo_url>

Example:

git clone https://github.com/user/project.git
🔹 3. Check Status
git status

Shows:

Modified files

Staged files

Untracked files

🔹 4. Add (Staging Area)
git add file.txt
git add .
🔹 5. Commit
git commit -m "Commit message"

Shortcut (tracked files only):

git commit -am "Quick commit"
🔹 6. Branching
git branch                # list branches
git branch feature-login  # create branch
git switch feature-login  # switch branch
git switch -c new-branch  # create + switch

Old method:

git checkout branch-name
🔹 7. Merge
git switch main
git merge feature-login
🔹 8. Remote Commands
git remote -v
git remote add origin <repo_url>
git push -u origin main
git pull origin main
git fetch
🔹 9. View History
git log
git log --oneline
git log --graph --oneline --all
🔹 10. Compare Changes
git diff
git diff branch1 branch2
🔹 11. Undo Changes

Unstage file:

git restore --staged file.txt

Discard changes:

git restore file.txt

Undo last commit (keep changes):

git reset --soft HEAD~1

Hard reset:

git reset --hard HEAD~1
🔹 12. Remove Files
git rm file.txt
🔹 13. Stash (Temporary Save)
git stash
git stash list
git stash pop
🔥 Basic Workflow (Daily Use)
