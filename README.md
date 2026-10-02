<p align="center"><img src="assets/fathom-header-banner.svg" alt="Fathom Works — homelable-mcp" width="100%"></p>

# `$ homelable-mcp`

**Lets an AI assistant look at and manage your home server map in [Homelable](https://github.com/Pouzor/homelable).** It offers 11 tools and 5 resources for that.

*A [Fathom Works](https://github.com/Jemplayer82) project.*

**In plain terms:** Homelable draws a map of the devices in your home lab. This small service is a bridge. It lets an AI assistant read that map and change it for you. MCP (Model Context Protocol) is the plug-in standard that lets an AI assistant use outside tools.

## `[ quick start ]`

This service is part of the `mcp-shared` Portainer stack. It runs on port 3111. Your AI client connects to these two addresses:

```
http://<host>:3111/mcp  # MCP endpoint
http://<host>:3111/health  # health check
```

Send an `x-api-key` header with every request except `/health`.

## `[ configuration ]`

Set these as environment variables, or in a `.env` file.

| Variable | What it does | Default |
|---|---|---|
| `MCP_API_KEY` | Key your AI client must send in `x-api-key` | `mcp_sk_changeme` |
| `MCP_SERVICE_KEY` | Key this service uses to talk to the Homelable backend | `svc_changeme` |
| `BACKEND_URL` | Address of the Homelable backend | `http://backend:8000` |

Change both keys before you use this for real.

## `[ license ]`

No license file is included in this repo.

<img src="assets/fathom-footer-banner.svg" alt="Fathom Works — sound the depths before you set a course" width="100%">
