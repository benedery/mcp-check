# MCP-Check Repository

This repository is designed to test and demonstrate the Model Context Protocol (MCP) GitHub functionality.

## Setup

To use MCP commands, you need to:

1. Install the MCP GitHub server:
```bash
npx -y @modelcontextprotocol/server-github
```

2. Configure your GitHub token in `~/.cursor/mcp.json`:
```json
{
    "mcpServers": {
      "github": {
        "command": "npx",
        "args": [
          "-y",
          "@modelcontextprotocol/server-github"
        ],
        "env": {
          "GITHUB_PERSONAL_ACCESS_TOKEN": "your_token_here"
        }
      }
    }
}
```

## Available MCP Commands

Here are some of the key MCP commands for GitHub:

### Repository Management
- Create repository
- Fork repository
- Search repositories
- Create/update files
- Create branches

### Issues and PRs
- Create issues
- Create pull requests
- Review pull requests
- Merge pull requests
- Get PR status
- List PR files

### Content Management
- Get file contents
- Push multiple files
- Search code
- List commits

### Collaboration
- Create issues
- Add comments
- Search users
- Update issues

## Testing Status

This repository serves as a test bed for verifying MCP command functionality. Each command can be tested to ensure proper integration with GitHub's API.

## Notes

- Make sure the MCP server is running (you should see "GitHub MCP Server running on stdio")
- Verify your GitHub token has the necessary permissions
- Keep your token secure and never commit it to version control