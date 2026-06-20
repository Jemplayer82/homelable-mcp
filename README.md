# homelable-mcp

MCP server for [Homelable](https://github.com/Pouzor/homelable) homelab topology management.

Exposes 11 tools and 5 resources for AI-assisted homelab management via the Model Context Protocol.

## Deployment

Part of the `mcp-shared` Portainer stack. Runs on port 3111.

```
http://<host>:3111/mcp  # MCP endpoint
http://<host>:3111/health  # health check
```

Auth: `x-api-key` header required on all requests except `/health`.
