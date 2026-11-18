# Caura

Caura gives Claude shared, governed memory for your team. Claude recalls what
your team already decided before it starts a task, follows the rules your
organization set for its agents, and saves decisions and outcomes so the next
session, or the next teammate, starts informed.

## What's included

- **Caura connector** (`https://caura.ai/mcp`): the `caura_*` tools for
  recall, writing memories, team rules, documents and the entity graph.
- **`caura-memory` skill**: tells Claude when to recall, what is worth saving,
  and how to treat recalled content.
- **Commands**: `/caura-ai:recall <topic>` and `/caura-ai:remember <text>`.

## Set up

1. Create a free account at [caura.ai](https://caura.ai).
2. Install the plugin and connect the Caura connector.
3. Ask Claude "what do we know about <a project>?" or run `/caura-ai:recall`.

The first time Claude uses Caura, your browser opens caura.ai to sign in. You
choose the tenant this Claude works in and approve it; Claude gets its own
agent, named after you (for example `claude-dana`). Revoke the connection any
time in caura.ai under Connect › Keys, where it is listed as "OAuth: Claude Code"
or "OAuth: Claude". Changing your Caura password also ends it.

## Data

The plugin sends data only to your Caura account at `caura.ai`:

- the search queries Claude makes when it recalls memories;
- the text of memories and documents Claude saves, and the outcomes it
  reports;
- the sign-in token caura.ai issued for this connection, to authenticate;
- a `X-Caura-Source: claude-plugin` header, so Caura can count connections
  made through this plugin. It carries nothing about you.

Caura stores saved memories in your organization's account, under your
organization's access rules, until you delete them. The plugin itself stores
nothing, runs no local programs and installs no hooks. See the
[privacy policy](https://caura.ai/legal/privacy/) and [terms](https://caura.ai/legal/terms/).

## Support

Open an issue in this repository or write to cs@caura.ai.

## License

Apache-2.0
