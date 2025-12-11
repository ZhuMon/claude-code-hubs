# claude-code-hubs

A Claude Code plugin repository containing MCP server configurations, custom slash commands, and skills.

## Installation

```bash
claude plugins:install github:ZhuMon/claude-code-hubs
```

## Features

### MCP Servers

This plugin automatically configures:

- **Serena** - Semantic code understanding with project memory and session persistence

### Skills

- **serena** - Usage guide for Serena MCP operations

## Contents

```
claude-code-hubs/
├── .claude-plugin/
│   └── plugin.json      # Plugin manifest with MCP server configs
├── skills/
│   └── serena/          # Serena usage skill
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

Test locally:

```bash
claude plugins:link /path/to/claude-code-hubs
```

## License

MIT
