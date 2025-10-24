```


Commit Types:


  feat – a new feature.
  fix – a bug fix.
  docs – documentation changes only.
  style – changes that do not affect logic, such as formatting or code style.
  refactor – code changes that neither fix a bug nor add a feature.
  perf – performance improvements.
  test – adding or updating tests.
  chore – maintenance tasks, build scripts, dependency updates, and similar.

  Examples:

  <type>(<scope>): <short summary>
  
  feat(model): implement baseline prediction
  feat(data): add dataset loader.


🔧 Setup & Configuration:

git init                               # Initialize a new Git repository
git clone <url>                        # Clone an existing repo from GitHub
git remote add origin <url>            # Connect your local repo to a GitHub repository
git remote -v                          # View all remote connections
git config --global user.name "Name"   # Set your global username
git config --global user.email "Email" # Set your global email
git config --list                      # Display all current Git settings


💾 Staging & Committing

git status                             # Show modified, staged, and untracked files
git add .                              # Stage all changes
git add <file>                         # Stage a specific file
git commit -m "message"                # Commit changes with a message
git commit --amend                     # Edit the last commit message
git restore <file>                     # Discard local changes in a file
git restore --staged <file>            # Unstage a file without deleting changes



🚀 Push & Pull

git push                               # Push local commits to GitHub
git push -u origin main                # First-time push (set main as default upstream)
git push origin <branch>               # Push a specific branch
git pull                               # Fetch and merge changes from GitHub
git fetch                              # Download changes without merging
git pull --rebase                      # Reapply your work on top of fetched commits


🌿 Branching

git branch                             # List all local branches
git branch -M main                     # Rename current branch to main
git checkout <branch>                  # Switch to an existing branch
git checkout -b <new-branch>           # Create and switch to a new branch
git switch <branch>                    # Alternative to checkout
git switch -c <new-branch>             # Create and switch to a new branch (modern syntax)
git branch -d <branch>                 # Delete a local branch
git push origin --delete <branch>      # Delete a remote branch


🧩 Merging & Rebasing

git merge <branch>                     # Merge another branch into the current one
git merge --abort                      # Abort a merge in progress
git rebase <branch>                    # Rebase current branch on top of another
git rebase --continue                  # Continue a rebase after resolving conflicts
git merge --squash <branch>            # Combine all commits from a branch into one


🧠 History & Viewing

git log                                # View commit history
git log --oneline                      # Condensed commit history (one line per commit)
git log --graph --oneline --decorate   # Visual branch and commit tree
git show <commit-id>                   # Show detailed info about a commit
git diff                               # Show unstaged changes
git diff --staged                      # Show staged changes
git diff HEAD                          # Compare working directory with last commit
git blame <file>                       # Show who last modified each line
git log -S "text"                      # Search for commits containing a specific string


🧹 Undo & Cleanup

git reset --soft HEAD~1                # Undo last commit but keep changes
git reset --hard HEAD~1                # Undo and delete last commit completely
git revert <commit-id>                 # Create a new commit that undoes a previous one
git clean -n                           # Preview which untracked files will be removed
git clean -f                           # Delete untracked files
git stash                              # Temporarily save uncommitted changes
git stash list                         # Show all saved stashes
git stash apply                        # Reapply last stash
git stash drop                         # Delete a stash


🧰 Useful Combos

git init && git add . && git commit -m "Initial commit" && git branch -M main && git remote add origin <url> && git push -u origin main  # Full project setup
git add . && git commit -m "Update" && git push                                            # Common workflow
git fetch origin && git rebase origin/main                                                 # Sync branch with latest main
git reset --hard origin/main                                                               # Discard local changes and reset
git pull origin main --allow-unrelated-histories                                           # Merge two unrelated repositories


```


    
