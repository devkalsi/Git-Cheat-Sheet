git config --list | findstr user    # Show git config, username

git init                 # Initialize a new repo
git clone <repo_url>     # Clone a remote repo
git status               # Check repo status
git diff                 # View unstaged changes
git diff --staged        # View staged changes

git add <file>           # Stage a file
git add .                # Stage all changes
git commit -m "message"  # Commit staged changes
git commit -am "msg"     # Stage + commit tracked files

git branch               # List branches
git branch <name>        # Create branch
git checkout <name>      # Switch branch
git branch -M main       # Renames current branch to 'main' (safe even if already 'main')
git branch --set-upstream-to=origin/main main #This tells Git: “my local main follows the remote main.”
git push -u origin main  # Sets upstream so future `git push` works without args

git remote -v            # List of any configured remote URLs
git remote add origin https://github.com/devkalsi/Git-Cheat-Sheet.git #Add Origin to remote
git fetch                # Fetch changes
git pull                 # Fetch + merge
git pull --rebase        #pull everything missing from remote main
git push --force         # Push update on already pushed commit
git push origin <branch> # Push branch


git log --graph --all
git blame <file>         # See who changed what
git show <commit>        # Show commit details


git reset --soft HEAD~1 # Undo commit, keep changes
git stash               # Save changes
git stash list          # View stashes
git stash apply         # Apply latest stash
git stash drop          # Delete stash