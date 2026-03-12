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

git remote -v            # View remotes
git remote add origin <url>
git fetch                # Fetch changes
git pull                 # Fetch + merge
git push --force         # Push update on already pushed commit
git push origin <branch> # Push branch


git log --graph --all
git blame <file>         # See who changed what
git show <commit>        # Show commit details


git reset --soft HEAD~1          # Undo commit, keep changes
git stash               # Save changes
git stash list          # View stashes
git stash apply         # Apply latest stash
git stash drop          # Delete stash