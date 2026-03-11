---
description: Run tests and fix failures
allowed-tools: Bash(npm test:*), Bash(pnpm test:*), Bash(pytest:*), Bash(go test:*), Bash(cargo test:*)
---

## Detect project

Try to run the project test suite.

!`npm test || pnpm test || pytest || go test ./... || cargo test`

## Task

If tests fail:

1. Analyze the error
2. Fix the code
3. Re-run tests until they pass
