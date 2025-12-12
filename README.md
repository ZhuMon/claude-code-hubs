# claude-code-hubs

A Claude Code plugin marketplace containing multiple plugins.

## Installation

Run in Claude Code:
```
/plugins marketplace add ZhuMon/claude-code-hubs
```

## Available Plugins

### serena

Serena MCP for semantic code operations, symbol manipulation, and project memory.

```
/plugins enable serena@zhumon-hubs
```

**Features:**
- Semantic code understanding
- Symbol manipulation (find, rename, replace)
- Project memory and session persistence

### commit

Smart git commit with conventional commits format.

```
/plugins enable commit@zhumon-hubs
```

**Features:**
- Conventional commits format (no emoji)
- Staged file detection
- Multi-concern split suggestions
- `--signoff` for DCO compliance

## Contents

```
claude-code-hubs/
├── .claude-plugin/
│   └── marketplace.json      # Marketplace definition
├── plugins/
│   ├── serena/               # Serena plugin
│   │   ├── plugin.json
│   │   └── skills/serena/
│   └── commit/               # Commit plugin
│       ├── plugin.json
│       └── skills/commit/
└── commands/                 # Shared slash commands
```

## Development

Run in Claude Code:
```
/plugins link /path/to/claude-code-hubs/plugins/serena
/plugins link /path/to/claude-code-hubs/plugins/commit
```

## License

MIT
