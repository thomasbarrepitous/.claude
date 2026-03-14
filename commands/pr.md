---
description: AI-generated Pull Request to main with safety check
allowed-tools: Bash(git add:*), Bash(git diff:*), Bash(git commit:*), Bash(git push:*), Bash(git status:*), Bash(git rev-parse:*), Bash(gh pr create:*)
---

!`git add .`

## Current Branch
!`git rev-parse --abbrev-ref HEAD`

## Repo status
!`git status`

## Staged changes
!`git diff --cached`

## Task

1. **Verify Branch:** Check if the current branch is `main`. If it is, **stop** and warn the user that a PR cannot be created from `main` to `main`. Suggest creating a feature branch.
2. **Analyze:** Examine the staged changes to understand the technical impact.
3. **Generate:** Create a **Conventional Commit message**.
   - Format: `type(scope): description`
   - Use a concise body for non-trivial changes.
4. **Propose:** Show the message and the PR action to the user for approval.

**If the user approves:**

1. `git commit -m "<generated_message>"`
2. `git push origin <current_branch>`
3. `gh pr create --base main --fill`

## Confirmation
Show the generated commit message and the **URL** of the newly created Pull Request.
