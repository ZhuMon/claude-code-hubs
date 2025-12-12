# claude-code-hubs

A Claude Code plugin repository containing MCP server configurations, custom slash commands, and skills.

## Installation

Run in Claude Code:
```
/plugins marketplace add ZhuMon/claude-code-hubs
/plugins enable hubs@zhumon-hubs
```

## Features

### MCP Servers

This plugin automatically configures:

- **Serena** - Semantic code understanding with project memory and session persistence

### Skills

- **serena** - Usage guide for Serena MCP operations
- **commit** - Smart git commit with conventional commits format (no emoji), staged file detection, and multi-concern split suggestions

## Contents

```
claude-code-hubs/
├── .claude-plugin/
│   └── plugin.json      # Plugin manifest with MCP server configs
├── skills/
│   ├── serena/          # Serena usage skill
│   └── commit/          # Git commit skill
├── commands/            # Custom slash commands
├── hooks/               # Hook configurations
└── settings/            # Configuration files
```

## Usage

After installation:

1. MCP servers are automatically available
2. Skills trigger based on context
3. Commands available with `hubs:` prefix

## Development

Run in Claude Code:
```
/plugins link /path/to/claude-code-hubs
```

## License

MIT
