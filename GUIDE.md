# Git and GitHub Basics: A Beginner's How-To Guide

## 1. What are Git and GitHub?

Git is a version-control tool that records changes to files over time. GitHub hosts Git repositories online and adds collaboration features such as pull requests, issues, and project boards.

## 2. Save a change with a commit

A commit is a saved snapshot in your local Git repository. In a terminal opened inside your project folder, use:

```bash
git status
git add README.md
git commit -m "Update README introduction"
```

Use `git status` to see which files changed. `git add` stages the file, and `git commit` records the staged changes locally.

## 3. Create a branch

A branch lets you work on a change without immediately changing the main branch.

```bash
git switch -c feature/add-guide-intro
```

Make and save your edits, then stage and commit them. Choose a branch name that describes the work.

## 4. Push your branch to GitHub

A push uploads your local commits to GitHub:

```bash
git push -u origin feature/add-guide-intro
```

A commit stays in your local repository until you push it. After pushing, GitHub can display the branch and its commits.

## 5. Open a pull request

On GitHub, open the repository and choose **Compare & pull request** for your branch. Give the pull request a clear title and explain what changed. Link the related issue by including text such as `Closes #1` in the description.

A pull request lets another person review the changes, ask questions, and request edits before they are merged into `main`.

## 6. Review and merge

The partner who did not create the pull request should check spelling, clarity, and technical accuracy. Leave a comment or request a change if needed. Once it is ready, merge the pull request into `main`.

After merging, the feature branch can be deleted on GitHub. To update a local copy of `main`, use:

```bash
git switch main
git pull
```

## 7. Work as a team

- Give each task an issue.
- Keep commits small and use clear messages.
- Use separate branches for separate tasks.
- Review pull requests before merging.
- Communicate before editing the same part of a file.

## 8. Merge conflicts

A merge conflict happens when Git cannot automatically combine changes to the same part of a file. Open the conflicted file and look for markers like:

```text
your version
partner's version
```

Edit the file so it contains the correct combined result, remove all conflict markers, then save and test it. Finish with:

```bash
git add README.md
git commit -m "Resolve README merge conflict"
```

For this assignment, both partners should edit the same file on different branches, create a conflict, resolve it together, and briefly document what was changed.

## Summary

Git records the history of a project. Branches allow separate work, pushes upload commits to GitHub, and pull requests provide a review step before changes are merged. These habits help teams collaborate while keeping the main branch organized. This guide helps beginners understand how to track changes, save commits, and collaborate through GitHub. Common Git commands include git add to stage changes, git commit to save changes, and git push to upload changes to GitHub. Main branch version: This guide explains Git basics for beginners. Conflict branch version: This guide teaches beginners how to use GitHub. Conflict branch version: This guide teaches Git basics and collaboration.
Git records the history of a project. Branches allow separate work, pushes upload commits to GitHub, and pull requests provide a review step before changes are merged. These habits help teams collaborate while keeping the main branch organized. This guide helps beginners understand how to track changes, save commits, and collaborate through GitHub. Common Git commands include git add to stage changes, git commit to save changes, and git push to upload changes to GitHub. Main branch version: This guide explains Git basics for beginners. Main branch version: This guide explains Git basics and collaboration.
