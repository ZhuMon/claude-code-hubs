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
  - `serena/` - Serena MCP usage guide
  - `commit/` - Git commit with conventional commits (no emoji)
- `mcp-configs/` - Backup MCP server configurations for quick restoration
- `.claude-plugin/plugin.json` - Plugin manifest (version, MCP servers)
- `.claude-plugin/marketplace.json` - Marketplace definition

## Installation

在 Claude Code 內執行：
```
/plugins marketplace add ZhuMon/claude-code-hubs
/plugins enable hubs@zhumon-hubs
```

## Local Development

在 Claude Code 內執行：
```
/plugins link /path/to/claude-code-hubs
```
