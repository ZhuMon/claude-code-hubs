# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

Claude Code plugin marketplace containing multiple plugins with MCP server configs and skills.

## Versioning

**IMPORTANT**: When adding or modifying plugin features, update the version in each plugin's `plugin.json`:

```json
{
  "version": "0.0.2",  // Increment this
  ...
}
```

## Structure

```
claude-code-hubs/
├── .claude-plugin/
│   └── marketplace.json          # Marketplace definition
└── plugins/
    ├── serena/                   # Serena MCP + skill
    ├── commit/                   # Commit skill
    ├── aws-doc/                  # AWS Documentation MCP
    ├── atlassian/                # Atlassian (Jira/Confluence) MCP
    └── langfuse-docs/            # Langfuse Documentation MCP
```

## Installation

在 Claude Code 內執行：
```
/plugins marketplace add ZhuMon/claude-code-hubs

# Skills
/plugins enable serena@zhumon-hubs        # Serena MCP + skill
/plugins enable commit@zhumon-hubs        # Commit skill

# MCP Servers (按需啟用)
/plugins enable aws-doc@zhumon-hubs       # AWS Documentation
/plugins enable atlassian@zhumon-hubs     # Jira/Confluence
/plugins enable langfuse-docs@zhumon-hubs # Langfuse Documentation
```

## Local Development

在 Claude Code 內執行：
```
/plugins link /path/to/claude-code-hubs/plugins/serena
/plugins link /path/to/claude-code-hubs/plugins/commit
```
