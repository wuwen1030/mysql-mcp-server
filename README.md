# MySQL MCP Server

A MySQL implementation of the Model Context Protocol (MCP) server. This server allows AI models to interact with MySQL databases through a standardized interface.

## Features

- List available database tables
- Get table schemas
- Execute read-only SQL queries
- Safe transaction handling with automatic rollback

## Installation

```bash
npm install
npm run build
```

## Usage

### Claude Desktop App

```
code ~/Library/Application\ Support/Claude/claude_desktop_config.json
```

```json

{
  "mcpServers": {
    "mysql": {
      "command": "node",
      "args": [
        "/ABSOLUTE/PATH/TO/PARENT/FOLDER/mysql-mcp-server/dist/index.js",
      ],
      "env": {
        "MYSQL_HOST": "127.0.0.1",
        "MYSQL_PORT": "3306",
        "MYSQL_USER": "root",
        "MYSQL_PASSWORD": "",
        "MYSQL_DATABASE": "test"
      }
    }
  }
}
```

Replace the env config with yours!

## License

MIT 