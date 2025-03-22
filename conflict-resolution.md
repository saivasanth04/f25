# Task 1 Deliverable: Version Control with Git

## Repository Overview
- **Repository URL:https://github.com/saivasanth04/f25.git
- **Purpose:** Demonstrate Git version control with branching and merge conflict resolution.

## Commit History
Run `git log --oneline` to see the commit history:

## Merge Conflict Resolution Steps
1. **Initialized Repository:**
   - Created a new Git repository with `git init`.
   - Added an initial `README.md` file with "# Task 1: Version Control Demo".
   - Committed with message "Initial commit: Add README".

2. **Created Branches:**
   - Created `feature-title` branch: Added "Title: Codtech DevOps Internship" to `README.md`.
     - Commit message: "Add title in feature-title branch".
   - Created `feature-subtitle` branch from `main`: Added "Subtitle: Learning Git Basics" to `README.md`.
     - Commit message: "Add subtitle in feature-subtitle branch".

3. **Merged First Branch:**
   - Switched to `main` and merged `feature-title` successfully using `git merge feature-title`.
   - Pushed changes to GitHub.

4. **Conflict Occurred:**
   - Attempted to merge `feature-subtitle` into `main` with `git merge feature-subtitle`.
   - Resulted in a merge conflict because both branches modified `README.md` after the initial line.

5. **Conflict Details:**
   - Before resolution, `README.md` showed:
Task 1: Version Control Demo
<<<<<<< HEAD Title: Codtech DevOps Internship
Subtitle: Learning Git Basics

"feature-subtitle"

6. **Resolution:**
- Manually edited `README.md` to combine both changes:
Task 1: Version Control Demo
Title: Codtech DevOps Internship
Subtitle: Learning Git Basics
- Staged the resolved file with `git add README.md`.
- Committed with message "Resolve merge conflict: Combined title and subtitle".
- Pushed the resolved `main` branch to GitHub.

7. **Added Documentation:**
- Created this `conflict-resolution.md` file to document the process.
- Committed with message "Add Task 1 deliverable documentation".
- Pushed to GitHub.

## Git Commands Used
- `git init`: Initialize the repository.
- `git checkout -b <branch>`: Create and switch to a new branch.
- `git add .`: Stage changes.
- `git commit -m "message"`: Commit changes with a message.
- `git merge <branch>`: Merge a branch into the current branch.
- `git push origin <branch>`: Push changes to the remote repository.

## Final Notes
- The repository demonstrates a clear commit history with branching and conflict resolution.
- All changes are visible on GitHub at https://github.com/saivasanth04/f25.git.
