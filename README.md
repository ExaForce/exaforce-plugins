# Exaforce Plugins

Official [Exaforce](https://www.exaforce.com) plugins for AI coding agents.

| Plugin | What it does |
|---|---|
| [`exaforce`](exaforce/) | Connects the agent to the Exaforce MCP server so you can search and investigate your Exaforce security data. |

## Install

Install from the Cursor Marketplace: open **Customize** in Cursor's sidebar, search for **Exaforce**, and
select **Install**.

To try a plugin from this repository before it is published, copy its folder to `~/.cursor/plugins/local`
and run **Developer: Reload Window**.

## Repository layout

- `.cursor-plugin/marketplace.json` lists every plugin in this repository.
- Each plugin lives in its own folder with a `.cursor-plugin/plugin.json` manifest, its components (for
  example `mcp.json`), and a `README.md`.

To add a plugin, create its folder, add an entry to `.cursor-plugin/marketplace.json`, and test it locally
before opening a pull request. Never commit secrets: the Cursor team reviews every change, and this
repository is public.
