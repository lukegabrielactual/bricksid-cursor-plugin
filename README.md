# BricksID Cursor Plugin

One-click install of the [BricksID](https://bricksid.com) remote MCP for Cursor and Grok Bot. Identify LEGO minifigs and sets from photos, and manage your BricksID collection from chat.

## What it does

- Packages the hosted BricksID MCP at `https://bricksid.com/mcp`
- Lets the agent scan photos of minifigs/sets, confirm BrickLink IDs, and update your collection
- No local MCP process, no API keys in the plugin, and no secrets in this repo

## Install from the marketplace

1. Open Cursor → **Plugins** / marketplace
2. Find **BricksID** (`bricksid`) and install
3. The plugin registers the remote MCP server automatically

Until marketplace listing is live, you can also point Cursor at this plugin directory or clone the repo and install from source.

## Connect / auth

BricksID uses browser login — **Google, Apple, or email**. When the agent first needs your account:

1. Follow the auth / connect flow prompted by the BricksID MCP tools
2. Sign in in the browser with Google, Apple, or email
3. Return to Cursor / Grok Bot; your session is tied to that login

This plugin does **not** store passwords, tokens, or API keys. Do not put credentials in config files.

## Plans

A **free BricksID account** is required to use the MCP. Paid plans may unlock higher limits or extra features on [bricksid.com](https://bricksid.com) — check the site for current pricing.

## Full MCP docs

See **https://bricksid.com/mcp** for tool reference, capabilities, and connection details.

## Repository layout

```text
bricksid-cursor-plugin/
├── .cursor-plugin/plugin.json
├── mcp.json
├── skills/connect-bricksid/SKILL.md
├── assets/logo.png (and logo.svg)
├── README.md
├── LICENSE
└── .gitignore
```

## License

MIT © 2026 BricksID / Luke Reiser
