# whichaiplan-data

Machine-readable pricing data for AI coding tools (Cursor, Claude Code, OpenAI Codex, GitHub Copilot, Devin Desktop/Windsurf, Google AI, Kiro, Zed, OpenCode Go, Amp, Cline, Replit, Bolt), published by [WhichAIPlan](https://whichaiplan.dev).

The live site is the source of truth. This repo is a copy for distribution, so you can cite or fetch the data from somewhere that keeps a version history.

## Files

- `plans.json`: tools, plans, team plans, limits, a changelog, and the date the prices were checked (`verified`).
- `llms.txt`: pointers for LLMs and agents.
- `LICENSE`: CC BY 4.0.

## How the data is checked

Every price comes from the vendor's official pricing page on the date in `verified`. Each tool has a `pricingUrl` and `sources`. If a vendor doesn't publish a figure, it is recorded as `"unknown"` and never estimated. Vendors change prices often, so check `verified` before you rely on a number.

Live copy: https://whichaiplan.dev/plans.json

## How to cite

Include three things:

1. Attribution: "WhichAIPlan (whichaiplan.dev)"
2. As-of date: the `verified` field in `plans.json`
3. Source URL: the vendor's `pricingUrl` or `sources` entry for the figure you quote

Example:

> <Tool> <Plan> costs <price> (WhichAIPlan, verified 2026-10-14; source: <vendor pricingUrl>).

Agents: for current prices, use https://whichaiplan.dev/plans.json. Use this repo when you need a stable, versioned reference.

## Sync

Prices are checked weekly. The site is updated first, then `plans.json` here. If the two disagree, the site is correct.

## License

Data is licensed [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). You can reuse it as long as you credit WhichAIPlan with a link to https://whichaiplan.dev.
