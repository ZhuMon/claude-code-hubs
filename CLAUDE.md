# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a Claude Code plugin repository designed for the marketplace. It stores Claude Code configurations, slash commands, skills, and related settings that can be installed via the plugin system.

## Plugin Structure

```
claude-code-hubs/
├── commands/           # Slash command definitions (.md files)
├── skills/             # Skill definitions for the Skill tool
├── hooks/              # Hook configurations
├── settings/           # Settings and configuration files
└── CLAUDE.md           # This file
```

## Creating Slash Commands

Place `.md` files in the `commands/` directory. Each file becomes a slash command where:
- Filename becomes command name (e.g., `review.md` → `/review`)
- File content is the prompt template
- Use `$ARGUMENTS` placeholder for user input

## Creating Skills

Skills extend Claude's capabilities. Place skill definitions in `skills/` directory following the skill format with:
- `name`: Skill identifier
- `description`: When to activate the skill
- Content: Instructions and resources for the skill

## Publishing to Marketplace

1. Push repository to GitHub
2. Install as plugin: `claude plugins:install github:username/claude-code-hubs`
3. Commands appear with prefix: `/hubs:command-name`

## Local Development

Test locally by symlinking to Claude Code's plugin directory or using `claude plugins:link`.
