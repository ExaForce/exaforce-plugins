# Exaforce

Connects Cursor to the Exaforce MCP server so you can search and investigate your Exaforce data from the
agent: identities, cloud resources, sessions, events, threat findings and cases. It uses the same tools
and system prompts as Exabot Search in the Exaforce Console.

The tools you see depend on what your tenant has onboarded. A tool appears only when the data source or
integration it relies on is configured for your tenant.

## Requirements

- An Exaforce tenant and a user account on it.

## Install and sign in

1. In Cursor, open **Customize** in the sidebar.
2. Search for **Exaforce**, select **Install**, and choose a project or user scope.
3. When Cursor asks you to authenticate the `exaforce` MCP server, start the sign-in. A browser window
   opens.
4. Enter your tenant name, and click **Next**. For `https://example.us.app.exaforce.io`, the tenant name
   is `example`.
5. Sign in with your usual Exaforce credentials.

No API token is needed, and this plugin stores no credentials.

## Access

The plugin reaches only your own tenant's data. Your Exaforce roles decide what you can read or change,
exactly as in the Exaforce Console.

## Example prompts

- "Who accessed the production AWS account in the last 24 hours?"
- "Show me all failed login attempts for user john.doe this week."
- "Summarize the open critical cases."

## Other MCP clients

Any client that supports remote MCP servers with OAuth can use the same server URL:
`https://mcp.api.us.app.exaforce.io`.

## Develop locally

To try a change before it is published, copy this repository to `~/.cursor/plugins/local/exaforce` and run
**Developer: Reload Window** in Cursor.

This repository is public, and every change is reviewed before it reaches Cursor users. Never commit
secrets.

## Support

Contact `support@exaforce.com`. Exaforce customers can also read the
[Exaforce MCP Server guide](https://docs.exaforce.com/how-to-and-extended-concepts/platform/mcp-exabot-search/mcp-exabot-search)
(sign-in required).
