# NextGenAi plugins for Claude Code

Claude Code plugins for Israeli businesses, made by [NextGenAi](https://next-gen.live). Each plugin is a set of [Agent Skills](https://code.claude.com/docs/en/skills). The site page about them is at https://next-gen.live/claude-skills/.

| Plugin | Skills | What it does |
|---|---|---|
| `hebrew-business` | quote-proposal, weekly-report, customer-reply | Hebrew price quotes and proposals, weekly reports from Excel or CSV, customer replies |
| `hebrew-copy` | hebrew-copy-check | Fixes Hebrew copy: RTL numbers, voice, machine-written tells, calls to action |
| `site-seo` | page-seo-geo, site-launch-check | Keywords, descriptions and FAQ for each page (SEO and GEO), plus a launch checklist |
| `daily-assistant` | daily-briefing, receipt-finder | Morning briefing from Calendar and Gmail, plus a receipt and invoice finder (needs the Gmail and Calendar connectors) |

## Install

In Claude Code:

```text
/plugin marketplace add yossiheinebiz-cloud/nextgenai-claude-plugins
/plugin install hebrew-business@nextgenai-plugins
```

Or from your shell:

```bash
claude plugin install hebrew-copy --marketplace yossiheinebiz-cloud/nextgenai-claude-plugins
```

You run a skill as `/<plugin>:<skill>`, for example `/hebrew-business:quote-proposal`. Claude also uses a skill on its own when a request matches its description.

## Safety

These plugins contain only instructions (SKILL.md files): no scripts, hooks or MCP servers. `daily-assistant` reads Gmail and Calendar through connectors you set up yourself. Its skills are written to be read-only and never send email. Read a skill before you install it.

## Licence

MIT. Send feedback and requests through https://next-gen.live/contact/
