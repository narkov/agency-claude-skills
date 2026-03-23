# Agency Toolkit — Claude Code Plugin Marketplace

A collection of Claude Code skills for digital agencies that build websites, run advertising, and manage SEO.

## Plugins

### 🔍 SEO (`/plugin install seo@agency-toolkit`)
- `/site-audit` — comprehensive SEO audit for a client website
- `/keyword-research` — keyword research with volume, difficulty, and intent clustering
- `/backlink-gap` — find backlink opportunities vs competitors (with spam filtering)
- `/content-gap` — find content topics competitors rank for but you don't

### 📊 Advertising (`/plugin install advertising@agency-toolkit`)
- `/ga4-report` — GA4 traffic and conversion report with period comparison
- `/ad-performance` — paid campaign analysis by campaign, landing page, device
- `/conversion-check` — quick daily check of ad clicks and conversions

### 🌐 Web Development (`/plugin install webdev@agency-toolkit`)
- `/launch-checklist` — pre-launch checklist (technical, SEO, performance, analytics, legal)
- `/agency-code-review` — code review focused on performance, SEO, accessibility
- `/page-speed` — performance analysis with optimization recommendations

### 📝 Notion Docs (`/plugin install notion-docs@agency-toolkit`)
- `/client-onboarding` — set up Notion workspace for a new client
- `/project-update` — update client project status and next steps
- `/meeting-notes` — create structured meeting notes with action items

### 📱 Telegram Reports (`/plugin install telegram-reports@agency-toolkit`)
- `/send-report` — format and send a client report to Telegram
- `/daily-digest` — daily summary of all clients' key metrics

### 👥 Client Management (`/plugin install client-management@agency-toolkit`)
- `/monthly-report` — comprehensive monthly report (SEO + Ads + Web)
- `/health-check` — quick health scan across all active clients
- `/client-brief` — generate structured brief from discovery call notes

## Installation

```bash
# Add the marketplace
/plugin marketplace add narkov/agency-claude-skills

# Install all plugins
/plugin install seo@agency-toolkit
/plugin install advertising@agency-toolkit
/plugin install webdev@agency-toolkit
/plugin install notion-docs@agency-toolkit
/plugin install telegram-reports@agency-toolkit
/plugin install client-management@agency-toolkit
```

## Requirements

These skills work best with the following MCP servers connected:
- **SE Ranking API** — for SEO data (audits, keywords, backlinks)
- **GA4** — for traffic and conversion data
- **Notion** — for documentation and project management
- **Telegram** — for report delivery

## License

MIT
