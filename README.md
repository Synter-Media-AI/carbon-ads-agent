# Carbon Ads MCP Starter Kit — Manage Carbon Ads with AI

> **This is a recipe repo.** The Synter MCP server itself lives at [Synter-Media-AI/mcp-server](https://github.com/Synter-Media-AI/mcp-server): 19 ad platforms, campaign creation on 14, one-click install in Cursor, Claude, ChatGPT, and VS Code. Issues, releases, and ⭐ go there.

[![MCP Compatible](https://img.shields.io/badge/MCP-compatible-blue)](https://modelcontextprotocol.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform: Carbon Ads](https://img.shields.io/badge/Platform-Carbon%20Ads-000000)](https://www.carbonads.net)

**Buy and sell developer inventory where engineers actually read.** Open this repo in Amp, Cursor, or VS Code and manage Carbon Ads campaigns with AI — contextual placements on Stack Overflow, engineering blogs, and docs sites, planned and reported through the Synter MCP server.

---

## Why Carbon Ads + AI?

Carbon Ads is the default buy for developer-facing SaaS: native units on Stack Overflow, CSS-Tricks-class blogs, newsletters, and documentation. Unlike consumer social, Carbon inventory sits next to code, RFCs, and tutorials — high-intent readers who ignore banner networks but click tools that solve the problem on the page.

The catch is operational. Buyers juggle site lists, creative sizes, flight dates, and “does this look like a sponsor or spam?” quality. An AI agent connected via MCP can draft a flight, compare Carbon vs EthicalAds vs Brave, and pull performance without another ad-ops console.

**Best for:** developer tools, APIs, cloud, observability, security, IDE extensions, B2B SaaS selling to engineers.

---

## Developer ad platforms compared

| Network | Typical inventory | Tracking posture | Best for |
|--------|-------------------|------------------|----------|
| **Carbon Ads** | Stack Overflow, developer blogs, newsletters | Contextual + standard advertiser pixels | Dev-tool demand on high-traffic blogs |
| **EthicalAds** | Read the Docs, PyPI-adjacent OSS, privacy publishers | No third-party cookies | Privacy-first open-source audiences |
| **Brave Ads** | Brave search, new tab, browser notifications | Privacy-preserving / BAT | Privacy-conscious developers and power users |

Use this kit for Carbon. Companion kits: [ethical-ads-agent](https://github.com/Synter-Media-AI/ethical-ads-agent), [brave-ads-agent](https://github.com/Synter-Media-AI/brave-ads-agent).

---

## Quick Start (30 Seconds)

### Amp / Cursor / VS Code (Copilot)

1. **Get a free API key** at [syntermedia.ai/developer](https://syntermedia.ai/developer)
2. **Set the key:**
   ```bash
   export SYNTER_API_KEY=syn_your_key_here
   ```
3. **Open this repo** in your editor
4. **Start chatting** — MCP tools are pre-configured in `.mcp.json`

### Claude Desktop

Copy `claude_desktop_config.json` to your Claude config directory and replace the API key:

- **macOS:** `~/Library/Application Support/Claude/claude_desktop_config.json`
- **Windows:** `%APPDATA%\\Claude\\claude_desktop_config.json`

---

## What You Can Do

| Capability | Example |
|-----------|---------|
| **Plan a developer flight** | "Draft a 30-day Carbon campaign for our CLI observability tool" |
| **Inventory fit** | "Which Carbon placements make sense for a Python SDK?" |
| **Network comparison** | "Compare Carbon vs EthicalAds vs Brave for a $15k developer launch" |
| **Creative briefs** | "Write Carbon native copy that does not look like a generic SaaS banner" |
| **Budget splits** | "Split $8k/month across Carbon and EthicalAds by docs vs blog inventory" |
| **Performance** | "Pull last 14 days of Carbon spend, CTR, and assisted signups" |
| **Delivery QA** | "Validate this Carbon campaign structure for delivery issues" |
| **Geo / language** | "Limit this flight to US, UK, DE engineering readers" |

This kit talks to the **hosted Synter MCP** (`@synterai/mcp-server` / https://mcp.syntermedia.ai). Connect the relevant ad accounts at [syntermedia.ai/credentials](https://syntermedia.ai/credentials). It is not a first-party Carbon Ads API wrapper.

---

## Example Conversations

### 1. Launch a developer-tool flight

> **You:** We ship a TypeScript SDK. I want Carbon Ads, not Google Display.
>
> **Agent:** Carbon is the right default for SDK awareness. I will plan a contextual flight next to TS/JS docs and engineering blogs, with copy that names the job-to-be-done (typed APIs, fewer runtime surprises) instead of a generic “#1 developer platform” claim.
>
> Suggested split: 70% documentation-adjacent inventory, 30% high-traffic blogs. Creative: 1 value headline + 1 proof line (stars, latency, or “works with Next.js”). Connect Carbon at syntermedia.ai/credentials and I will create the campaign via Synter MCP.

### 2. Carbon vs EthicalAds vs Brave

> **You:** Should we buy Carbon, EthicalAds, or Brave for a privacy-sensitive database product?
>
> **Agent:** All three are developer-adjacent, different jobs.
> - Carbon: reach and classic blog/SO adjacency.
> - EthicalAds: OSS docs readers who opted into privacy-first ads.
> - Brave: browser/search users who already rejected the cookie web.
>
> For a privacy database, I would lead EthicalAds + Brave, keep a smaller Carbon test for docs-heavy blogs. I can open the matching recipe kits and set budgets in Synter.

### 3. Delivery check

> **You:** Validate my campaign structure for delivery issues.
>
> **Agent:** Checking flights, dates, creative sizes, and destination URLs through Synter MCP… I will flag missing UTM, mismatched sizes, and destinations that 404.

---

## FAQ

### Is there an MCP for Carbon Ads?
Yes — this recipe repo pre-configures the Synter MCP server so Amp, Cursor, VS Code, and Claude Desktop can plan and manage Carbon Ads through Synter. The server lives at [Synter-Media-AI/mcp-server](https://github.com/Synter-Media-AI/mcp-server).

### Does Synter replace the Carbon publisher/advertiser dashboard?
No. Synter is the agent layer. Connect credentials, then ask the agent to plan, launch, and report.

### Carbon vs Carbon Ads vs ethical alternatives?
“Carbon Ads” here means the developer advertising network (buy-side + sell-side developer inventory), not carbon offsets.

---

## Related Repos

- [carbon-ads-agent](https://github.com/Synter-Media-AI/carbon-ads-agent) — Carbon Ads / developer blog inventory
- [ethical-ads-agent](https://github.com/Synter-Media-AI/ethical-ads-agent) — EthicalAds privacy-first OSS inventory
- [brave-ads-agent](https://github.com/Synter-Media-AI/brave-ads-agent) — Brave Ads, search, and new-tab
- [twitch-ads-agent](https://github.com/Synter-Media-AI/twitch-ads-agent) — Twitch Ads for live gaming
- [discord-quests-agent](https://github.com/Synter-Media-AI/discord-quests-agent) — Discord Quests gamer acquisition
- [reddit-ads-agent](https://github.com/Synter-Media-AI/reddit-ads-agent) — Reddit community ads
- [google-ads-agent](https://github.com/Synter-Media-AI/google-ads-agent) — Search intent capture
- [meta-ads-agent](https://github.com/Synter-Media-AI/meta-ads-agent) — Facebook & Instagram reach
- [cross-platform-ads-agent](https://github.com/Synter-Media-AI/cross-platform-ads-agent) — Multi-channel management

---

## License

MIT — see [LICENSE](LICENSE) for details.

Built by [Synter](https://syntermedia.ai) · [Get API Key](https://syntermedia.ai/developer) · [Documentation](https://syntermedia.ai/docs)
