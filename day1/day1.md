#Day 1

## Git & Development Environment Setup

> [!NOTE]
> Authenticating to GitHub in the command line requires [personal access token]()

### git commands
#### git add
```
# Add a specific file
git add filename

# Add all changes in the current directory
git add .
```
#### git commit
```
# Commits the changes in the staging area to the repository
git commit -m "Commit message"
```
#### git push
```
# Pushes local commits to the remote repository
git push origin main
```
#### git pull
```
# Fetches changes from the remote repository and merges them into the local branch
git pull origin main
```
#### git branch
```
# List all branches
git branch

# Create a new branch
git branch new-branch

# Delete a branch
git branch -d branch-to-delete
```
#### git merge
```
# Merge the 'develop' branch into the current branch
git merge develop
```

### git commit convention
1.	Subject line under 50 characters, in imperative mood, start with a capital letter.
2.	Body separated by a blank line, wrapped at 72 characters, describing the reason for the changes.
3.	Footer for referencing issues (e.g., Closes #1234) or co-authors.
```
<type>[optional scope]: <short summary>
[BLANK LINE]
[optional detailed description or body]
[BLANK LINE]
[optional footer or references]
```
##### Category of the commit
- feat: A new feature.
- fix: A bug fix.
- docs: Documentation-only changes.
- style: Changes that do not affect the meaning of the code (whitespace, formatting, missing semicolons, etc.).
- refactor: A code change that neither fixes a bug nor adds a feature.
- perf: A code change that improves performance.
- test: Adding or correcting tests.
- build: Changes that affect the build system or external dependencies (e.g., npm, Gradle, etc.).
- ci: Changes to continuous integration configuration files or scripts.
- chore: Other changes that don’t modify application logic but are necessary for development (e.g., updating dependencies, minor config changes).