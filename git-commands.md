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

