Add MCP server(s) to Claude Code. Available: aws-doc, atlassian, langfuse-docs

Usage: /mcp-add <server-name> [server-name...]

Run the appropriate `claude mcp add` command for: $ARGUMENTS

Commands:
- aws-doc: `claude mcp add -s user -t stdio aws-doc -e FASTMCP_LOG_LEVEL=ERROR -e AWS_DOCUMENTATION_PARTITION=aws -- uvx awslabs.aws-documentation-mcp-server@latest`
- atlassian: `claude mcp add -s user -t sse atlassian https://mcp.atlassian.com/v1/sse`
- langfuse-docs: `claude mcp add -s user -t http langfuse-docs https://langfuse.com/api/mcp`
