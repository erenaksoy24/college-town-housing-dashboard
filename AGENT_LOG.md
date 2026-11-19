# Agent log

Add a dated entry each time you work with your AI coding agent, with the newest entry at the bottom. Each entry records what you asked the agent, what it produced, and what you checked or changed. Paste your key prompts in exactly as you typed them. Include at least one time the agent got something wrong, and how you caught it.

Copy this outline for each entry:

```markdown
## YYYY-MM-DD: What you worked on

- **Asked:** "Paste your prompt here."
- **Agent produced:** What it made or changed.
- **Checked or changed:** How you checked it, and what you fixed.
```

## 2026-11-19: Add city filter to housing dashboard

- **Asked:** "Pull the latest main first. Read AGENTS.md and docs/data_description_sheet.md. Add an interactive city dropdown filter that allows users to select a specific city or view all cities. Update the summary statistics based on the selected city. Keep the existing bar chart, website design, data source, and $10,000 exclusion rule. Test the filter and document our AI-assisted work in AGENT_LOG.md."
- **Agent produced:** Fast-forwarded the dashboard branch to the latest `origin/main`, added a city selector that updates the sales count, median and average for the selected city, preserved the all-city median bar chart and source citation, and kept the $10,000 minimum sale price rule. Replaced the external CSV parser dependency with a quote-aware browser parser so the CSV loads when external scripts are unavailable.
- **Checked or changed:** Opened the page in headless Chromium and selected Davis, CA, then returned to All cities. The all-city view showed 35,402 qualifying sales, a $410,000 median and a $509,951 average; Davis showed 941 qualifying sales, an $889,000 median and a $976,896 average; returning to All cities restored the initial figures. Independently computed Davis's figures from the CSV and confirmed the bar chart remained present.
