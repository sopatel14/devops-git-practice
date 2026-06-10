# Git Commands Reference

## Setup & Config

### git --version

**What it does:** Displays the installed Git version.

```bash
git --version
```

### git config --global user.name

**What it does:** Sets your Git username.

```bash
git config --global user.name "Sourav Patel"
```

### git config --global user.email

**What it does:** Sets your Git email address.

```bash
git config --global user.email "souravpatel65@gmail.com"
```

### git config --list

**What it does:** Shows current Git configuration.

```bash
git config --list
```

---

## Basic Workflow

### git init

**What it does:** Initializes a new Git repository.

```bash
git init
```

### git add

**What it does:** Adds files to the staging area.

```bash
git add git-commands.md
```

### git add .

**What it does:** Stages all changes.

```bash
git add .
```

### git commit

**What it does:** Saves staged changes to repository history.

```bash
git commit -m "Add Git command reference"
```

---

## Viewing Changes

### git status

**What it does:** Shows the current repository state.

```bash
git status
```

### git log

**What it does:** Shows commit history.

```bash
git log
```

### git log --oneline

**What it does:** Displays compact commit history.

```bash
git log --oneline
```

### git diff

**What it does:** Shows unstaged changes.

```bash
git diff
```

## Branching Commands

### git branch

**What it does:** Lists all local branches and highlights the current branch.

```bash
git branch
```

### git branch <branch-name>

**What it does:** Creates a new branch without switching to it.

```bash
git branch feature-1
```

### git switch <branch-name>

**What it does:** Switches from the current branch to another existing branch.

```bash
git switch feature-1
```

### git switch -c <branch-name>

**What it does:** Creates a new branch and immediately switches to it.

```bash
git switch -c feature-2
```

### git branch -d <branch-name>

**What it does:** Deletes a local branch that has already been merged.

```bash
git branch -d feature-2
```

### git push -u origin <branch-name>

**What it does:** Pushes a branch to GitHub and sets the upstream tracking branch.

```bash
git push -u origin feature-1
```

## Advanced Git Commands (Merge, Rebase, Stash & Cherry-Pick)

### git merge <branch-name>

**What it does:** Merges another branch into the current branch.

```bash
git merge feature-login
```

### git merge --squash <branch-name>

**What it does:** Combines all commits from a branch into a single commit before merging.

```bash
git merge --squash feature-profile
```

### git rebase <branch-name>

**What it does:** Replays the current branch commits on top of another branch, creating a cleaner history.

```bash
git rebase main
```

### git log --oneline --graph --all

**What it does:** Displays a compact visual representation of commit history across all branches.

```bash
git log --oneline --graph --all
```

### git log --oneline --graph --all --decorate

**What it does:** Displays commit history along with branch names, tags, and HEAD references.

```bash
git log --oneline --graph --all --decorate
```

### git stash

**What it does:** Temporarily saves uncommitted changes and restores a clean working directory.

```bash
git stash
```

### git stash push -m "<message>"

**What it does:** Saves uncommitted changes with a descriptive message.

```bash
git stash push -m "login work"
```

### git stash list

**What it does:** Lists all saved stashes.

```bash
git stash list
```

### git stash pop

**What it does:** Restores the latest stash and removes it from the stash list.

```bash
git stash pop
```

### git stash apply

**What it does:** Restores a stash without removing it from the stash list.

```bash
git stash apply
```

### git stash apply stash@{n}

**What it does:** Restores a specific stash from the stash list.

```bash
git stash apply stash@{1}
```

### git cherry-pick <commit-hash>

**What it does:** Applies a specific commit from another branch to the current branch.

```bash
git cherry-pick 4a2f111
```

### git rebase --continue

**What it does:** Continues the rebase process after resolving conflicts.

```bash
git rebase --continue
```

git reset --mixed HEAD~1

**What it does:** Removes the latest commit and unstages the changes while keeping them in the working directory.

git reset --mixed HEAD~1
git reset --hard HEAD~1

**What it does:** Removes the latest commit and permanently deletes all associated changes.

git reset --hard HEAD~1
git reset HEAD <file>

**What it does:** Unstages a file without removing any changes from the working directory.

git reset HEAD notes.md
git revert <commit-hash>

**What it does:** Creates a new commit that reverses the changes introduced by a previous commit.

git revert abc1234
git reflog

**What it does:** Displays a history of all HEAD movements and reference updates, including resets, rebases, and recoverable commits.

git reflog

This matches the exact format of your existing `git-commands.md` sections.


GitHub CLI Commands

## gh auth login

**What it does:** Authenticates GitHub CLI with your GitHub account.

```bash
gh auth login
```

---

## gh auth status

**What it does:** Displays the currently authenticated GitHub account and authentication status.

```bash
gh auth status
```

---

## gh auth logout

**What it does:** Logs out the current GitHub CLI session.

```bash
gh auth logout
```

---

## gh repo create

**What it does:** Creates a new GitHub repository directly from the terminal.

```bash
gh repo create my-repo --public --add-readme
```

---

## gh repo clone

**What it does:** Clones a GitHub repository using GitHub CLI.

```bash
gh repo clone sopatel14/devops-git-practice
```

---

## gh repo list

**What it does:** Lists repositories owned by the authenticated user.

```bash
gh repo list
```

---

## gh repo view

**What it does:** Displays repository details from the terminal.

```bash
gh repo view
```

---

## gh repo delete

**What it does:** Deletes a GitHub repository (requires delete_repo permission).

```bash
gh repo delete sopatel14/gh-test-repo
```

---

## gh issue create

**What it does:** Creates a new issue in the current repository.

```bash
gh issue create --title "Test Issue" --body "Created using GitHub CLI"
```

---

## gh issue list

**What it does:** Lists issues in the repository.

```bash
gh issue list
```

---

## gh issue view

**What it does:** Displays details of a specific issue.

```bash
gh issue view 1
```

---

## gh issue close

**What it does:** Closes an issue by issue number.

```bash
gh issue close 1
```

---

## gh pr create

**What it does:** Creates a pull request from the current branch.

```bash
gh pr create --fill
```

---

## gh pr list

**What it does:** Lists pull requests for a repository.

```bash
gh pr list
```

---

## gh pr view

**What it does:** Displays details of a pull request.

```bash
gh pr view
```

---

## gh pr diff

**What it does:** Shows changes included in a pull request.

```bash
gh pr diff 1
```

---

## gh pr checkout

**What it does:** Checks out a pull request locally.

```bash
gh pr checkout 1
```

---

## gh pr review

**What it does:** Reviews a pull request by approving, commenting, or requesting changes.

```bash
gh pr review 1 --approve
```

---

## gh pr merge

**What it does:** Merges a pull request from the terminal.

```bash
gh pr merge 1 --squash
```

---

## gh run list

**What it does:** Lists GitHub Actions workflow runs.

```bash
gh run list
```

---

## gh run view

**What it does:** Displays details of a workflow run.

```bash
gh run view <run-id>
```

---

## gh workflow list

**What it does:** Lists workflows configured in a repository.

```bash
gh workflow list
```

---

## gh workflow view

**What it does:** Displays details of a workflow.

```bash
gh workflow view <workflow-name>
```

---

## gh api

**What it does:** Makes raw GitHub API requests directly from the terminal.

```bash
gh api user
```

---

## gh gist create

**What it does:** Creates a GitHub Gist from a file.

```bash
gh gist create notes.txt
```

---

## gh gist list

**What it does:** Lists your GitHub Gists.

```bash
gh gist list
```

---

## gh release create

**What it does:** Creates a GitHub release and tag.

```bash
gh release create v1.0.0
```

---

## gh alias set

**What it does:** Creates a shortcut for frequently used GitHub CLI commands.

```bash
gh alias set prs "pr list"
```

---

## gh search repos

**What it does:** Searches GitHub repositories from the terminal.

```bash
gh search repos devops
```

