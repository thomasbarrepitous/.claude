# Claude Code Configuration

This directory contains my Claude Code CLI configuration files.

## Contents

- `settings.json` - User preferences and UI settings
- `plugins/config.json` - Plugin configuration
- `skills/` - Custom skills (if any)

## What's Not Included

For privacy and security reasons, the following are excluded via `.gitignore`:

- `history.jsonl` - Conversation history
- `debug/` - Debug logs with local file paths
- `file-history/` - Session-specific edit history
- `shell-snapshots/` - Shell environment snapshots
- `projects/` - Project-specific settings with local paths
- `todos/` - Agent task data
- `statsig/` - Analytics data

## Usage

To use this configuration:

1. Install [Claude Code](https://claude.com/claude-code)
2. Copy the relevant configuration files to your `~/.claude` directory
3. Adjust settings as needed for your environment

## More Information

For more details about Claude Code configuration, visit the [official documentation](https://docs.claude.com/claude-code).
