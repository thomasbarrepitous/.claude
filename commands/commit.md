---
description: AI commit with confirmation
allowed-tools: Bash(git add:*), Bash(git diff:*), Bash(git commit:*), Bash(git push:*), Bash(git status:*)
---

!`git add .`

## Repo status
!`git status`

## Staged changes
!`git diff --cached`

## Task

1. Analyze the staged changes.
2. Generate a **Conventional Commit message**.

Format:

type(scope): description

3. Show the message and ask for confirmation.

If approved run:

git commit -m "<message>"
git push
