# imagery (Claude Code plugin)

Connects Claude Code to the imagery.vision canvas open and signed in in your browser (Chrome or
Edge). Claude can then read, build and run workflows there; nodes appear as you talk.
Generations run in your browser session and are billed to your workspace as usual.

The plugin starts the local MCP server `imagery-mcp` with `npx` from docs.imagery.vision
(Node.js 20 or newer). It holds no credentials; the pairing code you pass at install time
(`--config pairing_token=…`, stored as a sensitive plugin option) only pairs it with your
browser tab.

```bash
claude plugin marketplace add sbauer-hash/imagery-claude-plugins
claude plugin install imagery@imagery-claude-plugins --config pairing_token=<pairing code>
```

Don't combine it with a `claude mcp add imagery …` entry, or every tool shows up twice.
Windows: not tested yet; use `claude mcp add` with `cmd /c npx` there
(https://docs.imagery.vision/editor/mcp/).
