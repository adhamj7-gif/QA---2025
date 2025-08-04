# Git & GitHub Team Workflow Practice

> A hands-on exercise set for students to master the collaborative feature development workflow using Git and GitHub.

This repository is designed to walk you through a full development cycle, from cloning a project to creating features, handling conflicts, and reviewing code.

---

## The Core Workflow

Follow this cycle for every new feature you build:

1.  **Sync with `main`**: Always start with the latest code.
    ```bash
    git checkout main
    git pull origin main
    ```

2.  **Create a Feature Branch**: Isolate your work from the main codebase.
    ```bash
    # Use a descriptive branch name
    git checkout -b feature/add-new-page
    ```

3.  **Develop & Commit**: Create your files and save your progress in small, logical commits.
    ```bash
    # After creating/editing files...
    git add .
    git commit -m "feat: Add cool new page"
    ```

4.  **Push your Branch**: Upload your new branch to GitHub.
    ```bash
    git push origin feature/add-new-page
    ```

5.  **Create a Pull Request (PR)**: On GitHub, open a pull request to merge your branch into `main`. Assign a teammate to review your code.

6.  **Review & Merge**: Your teammate will review the changes, leave comments, and approve. Once approved, merge the PR into `main`.

---

## Exercises

This project includes guided exercises to practice key skills:

*   **Exercise 1**: Initial Setup and First Commit
*   **Exercise 2**: Creating a Feature Branch (About Page)
*   **Exercise 3**: Pull Requests & Code Reviews
*   **Exercise 4**: Updating Your Branch with `rebase`
*   **Exercise 5**: Simulating & Resolving a Merge Conflict
*   **Exercise 6**: Adding a Shared Component (Footer)

---

## Key Commands Cheatsheet

| Command                       | Description                                            |
| :---------------------------- | :----------------------------------------------------- |
| `git clone <url>`             | Download a repository to your local machine.           |
| `git status`                  | Show the current status of your working directory.     |
| `git log --oneline --graph`   | View a condensed, visual history of your commits.      |
| `git fetch origin`            | Get updates from the remote repo without merging.      |
| `git rebase origin/main`      | Replay your commits on top of the latest `main` branch. |
| `git stash`                   | Temporarily save changes that are not ready to be committed. |
| `git branch -d <branch-name>` | Delete a local branch.                                 |

---

