# Git Commands Reference

A personal Git and GitHub command reference created while learning version control as part of my DevOps journey.

This repository contains commonly used Git and GitHub CLI commands along with explanations, examples, and practical notes collected through hands-on practice.

---

## About

The goal of this repository is to serve as a quick reference guide for:

* Git fundamentals
* Branching strategies
* Merging and rebasing
* Undoing changes safely
* Remote repository management
* GitHub CLI (gh)
* Pull requests and collaboration workflows

Rather than memorizing commands, this repository provides explanations and examples that can be used during real-world development and DevOps work.

---

## Topics Covered

### Git Basics

* Repository initialization
* Cloning repositories
* Tracking files
* Committing changes
* Viewing history

### Branching

* Creating branches
* Switching branches
* Listing branches
* Deleting branches

### Merging & Rebasing

* Merge workflows
* Rebase workflows
* Resolving conflicts

### Undo Operations

* git reset
* git revert
* git reflog
* Recovering lost commits

### Remote Repositories

* Adding remotes
* Pushing changes
* Pulling updates
* Fetching changes

### GitHub CLI (gh)

* Authentication
* Repository management
* Issues
* Pull requests
* Workflow management
* GitHub API usage

---

## Repository Structure

```text
git-commands/
├── git-commands.md
├── screenshots/
└── README.md
```

---

## Example Commands

### Check Repository Status

```bash
git status
```

### View Commit History

```bash
git log --oneline --graph --all
```

### Create a Branch

```bash
git checkout -b feature-branch
```

### Push Changes

```bash
git push origin main
```

### GitHub CLI Authentication

```bash
gh auth login
```

---

## Why This Repository?

Git is one of the most important tools for DevOps Engineers, Cloud Engineers, and Software Developers.

This repository acts as a personal knowledge base that can be referenced whenever needed and expanded over time as new workflows and commands are learned.

---

## Learning Outcomes

Through building this reference, I practiced:

* Git workflows
* Branch management
* Pull request workflows
* GitHub repository management
* GitHub CLI
* Collaboration best practices
* Version control troubleshooting

---

## Technologies Used

* Git
* GitHub
* GitHub CLI (gh)
* Linux (Ubuntu)

---

## Author

**Sourav Patel**

GitHub: https://github.com/sopatel14

---

## License

This repository is intended for educational purposes, learning, and reference.

