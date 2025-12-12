# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

Claude Code plugin marketplace containing MCP server configs, slash commands, and skills.

## Versioning

**IMPORTANT**: When adding or modifying plugin features, update the version in `.claude-plugin/plugin.json`:

```json
{
  "version": "0.0.2",  // Increment this
  ...
}
```

The `marketplace.json` uses `"latest"` and automatically picks up the version from `plugin.json`.

## Structure

- `commands/` - Slash commands (`.md` files, use `$ARGUMENTS` for input)
- `skills/` - Skill definitions
- `mcp-configs/` - Backup MCP server configurations for quick restoration
- `.claude-plugin/plugin.json` - Plugin manifest (version, MCP servers)
- `.claude-plugin/marketplace.json` - Marketplace definition

## Installation

```bash
claude plugins:install github:ZhuMon/claude-code-hubs
claude plugins:enable hubs@zhumon-hubs
```

## Local Development

```bash
claude plugins:link /path/to/claude-code-hubs
```
