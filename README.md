# Git Assignment

## Overview

This assignment is designed to provide practical experience with Git and GitHub by working through common version-control workflows. It covers repository creation, commits, branches, synchronization with remote repositories, pull requests, conflict handling, cherry-picking, resetting commits, and reverting changes.

The assignment is divided into five questions, with each question focusing on a different aspect of Git workflow and version management.

---

## Question 1: Repository Setup and Basic Git Workflow

The first question introduces the basic Git workflow.

The task begins with creating a new Git repository and adding a file to it. The changes made to the file are recorded as commits, allowing the project history to be tracked over time.

The assignment then requires viewing the repository's commit history to understand how Git records changes.

After the initial commit, the same file is modified again. The assignment demonstrates how Git identifies changes that have been made but have not yet been prepared for a commit. These changes are then staged and committed as a new version.

The final part of the question focuses on working with GitHub. The repository is cloned locally, changes made to the remote repository are fetched, and those changes are incorporated into the local repository.

### Concepts Covered

- Creating a Git repository
- Creating and tracking files
- Making commits
- Understanding commit history
- Identifying modified and unstaged changes
- Staging changes
- Cloning a GitHub repository
- Fetching remote changes
- Pulling and integrating remote changes

---

## Question 2: Feature Branch Workflow

The second question focuses on using branches to develop features separately from the main branch.

A new feature branch is created from the main branch and changes are made to the project within that branch. These changes are committed independently so that the main branch remains unaffected during development.

Once the feature is complete, the work is brought back into the main branch through a merge. The final changes are then synchronized with the remote repository.

This demonstrates a common development workflow where new features are developed independently and integrated into the main project after completion.

### Concepts Covered

- Creating feature branches
- Switching between branches
- Making isolated changes
- Committing branch-specific changes
- Merging a feature branch into the main branch
- Synchronizing merged changes with GitHub

---

## Question 3: Pull Requests and Merge Conflicts

The third question introduces a collaborative GitHub workflow using feature branches and pull requests.

A feature branch is created and changes are made to a project file. The changes are committed and pushed to the remote feature branch.

A pull request is then created to propose merging the feature into the main branch.

The assignment also simulates another user making changes to the same file directly in the main branch. Because both branches modify the same area of the file, a conflict occurs when the feature branch is integrated.

The conflict is resolved by bringing the latest main-branch changes into the feature branch and reconciling the conflicting modifications before completing the integration.

### Concepts Covered

- Feature-based development
- Remote feature branches
- Pull requests
- Collaborative development
- Conflicting changes
- Conflict resolution
- Rebase-based conflict handling

---

## Question 4: Cherry-Picking Specific Commits

The fourth question focuses on selectively applying individual commits from one branch to another.

Multiple changes are made to the same file on a feature branch, with each change recorded as a separate commit. The commit history is then examined to identify the specific commit that needs to be transferred.

Instead of merging the entire branch, only the selected commit is applied to another branch. This demonstrates how Git can reuse a specific piece of work without bringing all changes from the source branch.

The assignment also demonstrates that cherry-picking can result in a conflict when the selected commit is incompatible with the current state of the destination branch. The conflict is resolved before the selected change is successfully applied.

### Concepts Covered

- Creating multiple commits
- Identifying specific commits
- Selectively transferring changes between branches
- Cherry-picking
- Handling cherry-pick conflicts
- Continuing after conflict resolution

---

## Question 5: Reset and Revert

The fifth question demonstrates two different ways of dealing with previous commits: resetting and reverting.

Multiple commits are created on a feature branch. The commit history is then examined to select a particular point in the project's history.

The reset operation is used to move the current branch reference back to an earlier commit. This demonstrates how Git can move the branch's history to a previous state.

The assignment then introduces revert as a separate approach. Instead of removing a commit from the visible history, reverting creates a new commit that reverses the changes introduced by an earlier commit.

The final step compares the commit history after a reset with the history after a revert.

### Reset vs Revert

| Aspect | Reset | Revert |
|---|---|---|
| Purpose | Moves the branch back to an earlier commit | Reverses the effect of an existing commit |
| History | Can remove commits from the current branch history | Preserves the existing history |
| New commit created | Depends on the reset type; generally no new reversal commit | Yes |
| Best suited for | Rewriting local or private history | Safely undoing changes in shared history |
| Effect on commit history | Changes the branch's history | Adds a new commit that records the reversal |

The assignment demonstrates why understanding the difference between these operations is important when working with shared repositories.

---

## Learning Outcomes

After completing this assignment, the learner should understand the practical Git workflow involved in:

- Managing repositories and files
- Tracking changes through commits
- Reading commit history
- Working with local and remote repositories
- Creating and managing feature branches
- Merging feature work
- Working collaboratively through pull requests
- Identifying and resolving merge conflicts
- Selectively applying individual commits
- Understanding cherry-pick conflicts
- Moving a branch to an earlier point in history
- Reversing previously committed changes
- Understanding the difference between rewriting history and safely undoing changes

## Assignment Summary

This assignment progresses from fundamental Git operations to more advanced version-control scenarios. The first question establishes the basic repository and commit workflow. The second introduces feature branches and merging. The third moves into collaborative development and conflict resolution through pull requests. The fourth demonstrates selective commit transfer using cherry-picking. Finally, the fifth explores history management through reset and revert.

Together, these exercises provide a practical understanding of how Git can be used to manage code changes, collaborate with other developers, and safely control project history.
