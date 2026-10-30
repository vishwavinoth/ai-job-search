# Search Queries for Job Scraper

## Installed portal CLIs (primary for `/scrape`)

`/scrape` discovers every portal skill under `.agents/skills/*/SKILL.md` and runs its CLI first. Shipped country-agnostic CLIs include `linkedin-search` and `freehire-search`; Danish demos and any skill you add with `/add-portal` are included the same way. You do **not** need a matching `site:` line below for those CLIs to run.

The `site:` query templates in this file are the **WebSearch fallback** — for portals without a CLI, company career pages, or when a CLI fails.

**LinkedIn locations to run:** `Bengaluru, Karnataka, India`, `India`, `Remote`, `Singapore`, `Dubai, United Arab Emirates`, `Germany`, `Netherlands`, `Ireland`. Use each with the Priority 1 titles.

**Language scope:** write every query category in every language listed in your CLAUDE.md Languages table (typically 1-2, sometimes more). A posting requiring a language you have *not* declared, as a job condition, is excluded before scoring; a posting requiring a *higher level* than you declared in a language you *do* work in is flagged for your own judgment, not excluded — see `04-job-evaluation.md`'s Language Gate, the single source of truth for this rule. Translate each category's keywords rather than machine-translating word-for-word (e.g. "Frontend Developer" -> "Desarrollador Frontend", not a literal word-for-word translation) if you work in more than one language. Tech postings in Vishwa's target markets are written in English, so queries stay in English.

## Search Sites

India:
- **naukri.com** - India's largest general job board
- **hirist.tech** - India tech roles
- **cutshort.io** - India tech roles and startups
- **instahyre.com** - India tech roles
- **wellfound.com** - startups, India and global
- **linkedin.com/jobs** - also covered by `linkedin-search` CLI

Singapore:
- **mycareersfuture.gov.sg** - government job portal
- **sg.jobstreet.com** - general job board
- **nodeflair.com** - tech roles, shows salaries

Dubai / UAE:
- **naukrigulf.com** - Gulf job board
- **bayt.com** - Middle East job board
- **gulftalent.com** - Gulf professional roles

Europe and worldwide with visa sponsorship:
- **relocate.me** - tech jobs with relocation support
- **visasponsor.jobs** - jobs from visa-sponsoring employers
- **arbeitnow.com** - Germany, with a visa sponsorship filter
- **landing.jobs** - Europe tech roles
- **eures.europa.eu** - EU job portal

Remote:
- **remoteok.com**, **weworkremotely.com**, **himalayas.app** - keep only roles open to candidates in India

Secondary (company career pages via Google):
- Direct Google searches with `site:` filters for known target companies

## Query Categories

Queries are grouped by priority. Write **each category in every language from your Languages table** (see Language scope above). Combine each query with your location terms (e.g. your city, region, or metro area) where the site supports it.

**Organize by function, not job title.** The same underlying work carries different titles across companies and markets (a "Data Scientist" role at one employer may be posted as "Insights Analyst" or "Data Consultant" at another). Name each priority category after the function it covers, and list several plausible job titles as query variants within that category rather than betting an entire priority tier on one exact title string.

### Priority 1: Hands-on Full Stack Building

These match your strongest and most desired career direction.

```
site:naukri.com "Full Stack Developer" React Node.js Bengaluru
site:naukri.com "Full Stack Engineer" Next.js Bengaluru
site:hirist.tech "Full Stack Developer" React Node.js
site:wellfound.com "Full Stack Engineer" React Next.js India
site:linkedin.com/jobs "Full Stack Developer" Bengaluru India
site:mycareersfuture.gov.sg "Full Stack Developer" React
site:sg.jobstreet.com "Full Stack Developer" React Node.js
site:naukrigulf.com "Full Stack Developer" React Dubai
site:bayt.com "Full Stack Developer" React Dubai
site:relocate.me "Full Stack" React
site:visasponsor.jobs "Full Stack Developer"
site:arbeitnow.com "Full Stack" React visa sponsorship
```

### Priority 2: AI Engineering and Agents

These match your AI engineering direction.

```
site:naukri.com "AI Engineer" LLM Bengaluru
site:wellfound.com "AI Engineer" TypeScript India
site:linkedin.com/jobs "AI Engineer" "agents" Bengaluru
site:linkedin.com/jobs "Full Stack" "LLM" Singapore
site:relocate.me "AI Engineer"
site:himalayas.app "AI Engineer" TypeScript remote
site:remoteok.com "AI Engineer" LLM
```

### Priority 3: Solutions and Workflow Automation

Adjacent roles you could pivot into.

```
site:naukri.com "Solutions Engineer" Bengaluru
site:linkedin.com/jobs "Forward Deployed Engineer" India
site:linkedin.com/jobs "Automation Engineer" n8n
site:linkedin.com/jobs "Solutions Engineer" API Singapore
site:wellfound.com "Founding Engineer" React India
```

### Priority 4: Frontend and React Developer

Wider net for general technical roles.

```
site:naukri.com "React Developer" Next.js Bengaluru
site:naukri.com "Frontend Developer" React Bengaluru
site:hirist.tech "UI Developer" React
site:cutshort.io "Next.js Developer" Bengaluru
site:linkedin.com/jobs "Senior Frontend Engineer" React Singapore
site:naukrigulf.com "React Developer" Dubai
site:landing.jobs "Frontend" React
```

## Location Filter

When evaluating results, verify the job location against your target list. Define acceptable areas:
- Bengaluru (ideal)
- Remote roles open to candidates in India (ideal)
- Singapore, Dubai/UAE and Europe, with visa sponsorship (ideal)
- Any other country with visa sponsorship (acceptable)
- Abroad with sponsorship not stated (borderline - flag it and check the careers page)
- Other Indian cities (borderline - ask)
- Abroad with no sponsorship, or remote restricted to another country's residents (too far)

## Language Filter

Your working languages and levels are in CLAUDE.md's Languages table. When filtering scraped results, apply `04-job-evaluation.md`'s Language Gate: a posting requiring a language you haven't declared at all is excluded; a posting requiring a higher level than you declared in a language you do work in is not excluded, flag it clearly instead (see `job-scraper/SKILL.md`'s Step 3 "Quick Fit Assessment" for how the flag surfaces in `/scrape` output). Postings simply *written* in a language you don't work in, that don't require it on the job, are fine.

## Date Filter

Only include jobs posted within the last 14 days, or with an application deadline that has not yet passed. If a posting date cannot be determined, include it but flag as "date unknown".

## Adapting Queries

If the user specifies a focus area, select queries from the matching category and also generate 2-3 custom queries for that focus. For example:
- "/scrape [focus_area]" -> relevant category queries + custom focus-specific queries
