# imagery.vision plugins for Claude Code

Plugin marketplace for [imagery.vision](https://imagery.vision). The `imagery` plugin connects
Claude Code to the imagery.vision canvas open in your browser (Chrome or Edge), so Claude can
build and run workflows there.

```bash
claude plugin marketplace add sbauer-hash/imagery-claude-plugins
claude plugin install imagery@imagery-claude-plugins --config pairing_token=<pairing code>
```

The pairing code (Kopplungs-Code) is shown in imagery.vision on the **MCP connection** node.
Start a new session afterwards, then click the **MCP** chip in the imagery.vision header.
Requires Node.js 20 or newer.

Update:

```bash
claude plugin marketplace update imagery-claude-plugins
claude plugin update imagery@imagery-claude-plugins
```

Guide: https://docs.imagery.vision/editor/mcp/

This repository is generated: `imagery/` is copied from the imagery.vision source on every
release. Please report issues at https://github.com/sbauer-hash/imagery-vision/issues or via
imagery.vision support.
