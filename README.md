
GIT & GITHUB COMPLETE WORKFLOW (SSH)


PHASE 1: INITIAL SETUP & FIRST PUSH
----------------------------------------------------------
1. git init                               # Start local repo
2. git add .                              # Stage all files
3. git commit -m "Initial commit"         # Save snapshot
4. git remote add origin git@ssh-link
5. git pull origin main --rebase          # Sync with GitHub's README/License
6. git push -u origin main                # Upload to main branch

PHASE 2: WORKING ON A FEATURE BRANCH ("force")
----------------------------------------------------------
1. git checkout -b force                  # Create and switch to 'force'
2. git add .                              # Stage changes
3. git commit -m "Your message"           # Save changes
4. git pull origin force --rebase         # SYNC (Fixes the 'rejected' error)
5. git push -u origin force               # Upload to 'force' branch

PHASE 3: CREATING A PULL REQUEST (PR)
----------------------------------------------------------
1. Go to your repository
2. Click "Compare & pull request" (Yellow bar).
3. Check: [base: main] <- [compare: force].
4. Click "Create pull request".
5. Click "Merge pull request" -> "Confirm merge".

PHASE 4: SYNCING LOCAL MAIN
----------------------------------------------------------
1. git checkout main                      # Switch back to main
2. git pull origin main                   # Pull the merged code from GitHub
==========================================================
