# limena plugins

Official plugin marketplace for [limena](https://limena.app) — the accessibility audit your dev team will actually fix.

## Install in claude.ai

1. **claude.ai** → Customize → Personal plugins → **+** → Create plugin → **Add marketplace**
2. Pick **Add from a repository**
3. Paste this repo's URL:
   ```
   https://github.com/rshortux/limena-plugins
   ```
4. Install the **limena — accessibility audits** plugin
5. When prompted, paste your `lmn_…` API key (generate one at [console.limena.app/settings/api-keys](https://console.limena.app/settings/api-keys))

## What's in it

Currently one plugin:

| Plugin | What it does |
|---|---|
| **limena — accessibility audits** | Drives limena's hosted platform from Claude. Walks "which client → which program → which URLs" conversationally, then queues audits, polls, and summarises findings. Pairs axe-core with an LLM heuristic engine for ~96% WCAG 2.2 AA coverage. |

## Install in other agents

- **Claude Desktop / Cursor / Zed**: see [limena.app/connect](https://limena.app/connect) for the MCP config snippet.
- **Claude Code**: same page, plus the SKILL.md install.

## Security

Each connection uses a workspace API key with:

- Per-key **scopes** (read / write / admin) — mint read-only keys for browser-based connectors
- Optional **origin allowlist** for browser-based callers
- Configurable **rate limit** (default 100 req/min)
- **30-day usage log** per key for leak detection

Revoke any key at any time in **Settings → API keys** — calls stop in under a second.

## Support

- Email: `ryan@limena.app`
- Docs: [limena.app/connect](https://limena.app/connect)
- Issues with the plugin itself: open one on this repo

## License

MIT — see `LICENSE`.
