<!-- Title: CAURA-XXX- <what changes> (CAURA-000- when there is no ticket). -->

### What changes

### Checklist

- [ ] **Validated.** `claude plugin validate .` passes locally (CI runs it too).
- [ ] **Tried it.** Installed from this branch in Claude Code and called a `caura_*` tool, or say why not.
- [ ] **Docs.** README's "Set up" and "Data" sections still say what the plugin does and sends.
- [ ] **Names people see.** A renamed command, skill or setting is renamed in the README and in
      caura-enterprise's docs that mention the plugin, or their PR is linked here.
- [ ] **Connector.** `.mcp.json` still points at `https://caura.ai/mcp`, carries no key or secret,
      and sends `X-Caura-Source: claude-plugin` (CI checks this).
- [ ] **Version.** `version` in `.claude-plugin/plugin.json` is bumped if this ships to users.
- [ ] Commits are signed off (`git commit -s`).
