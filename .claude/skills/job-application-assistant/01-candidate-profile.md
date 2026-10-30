---
framework_version: 1.1.1
---

# Candidate Profile

## Identity
- **Name:** Vishwa R
- **Location:** Bengaluru, India
- **Phone:** +91 85248 40646
- **Email:** vishwa.js@outlook.com
- **LinkedIn:** https://www.linkedin.com/in/vishwaoffl
- **GitHub:** https://github.com/vishwavinoth
- **Portfolio:** https://vishwa.vercel.app
- **Status:** Employed - Full Stack Developer at Nexevo Technologies (since Oct 2023)
- **Constraints:** Bengaluru on-site/hybrid or remote. Open to relocating abroad (Singapore, Dubai/UAE, Europe, others) only with employer visa sponsorship.
- **CV language:** English

### Languages
<!-- Every language you can work in professionally, with your honest level. Used by the
Language Gate in 04-job-evaluation.md and by job-scraper/search-queries.md's query-language
generation. Omit any language you don't actually work in - an undeclared language is treated as
a hard no, not a gap to smooth over. -->

| Language | Level | Notes |
|----------|-------|-------|
| Tamil | Native | |
| English | Professional working proficiency | Working language; no test score on file |
| Kannada | Conversational | |

## Education

| Degree | Period | Institution | Key Topics |
|--------|--------|-------------|------------|
| B.Sc. Computer Science | 2019-2022 | Thanthai Hans Roever College, Perambalur, Tamil Nadu | Computer Science |

## Professional Experience

### Full Stack Developer - Nexevo Technologies (Oct 2023 - Present)
Bengaluru, India
- Owned product delivery end to end: scoping and PRDs with the sales team, then architecture, build, deployment and post-release support
- Worked with the sales team through pre-sales and scoping, turning client conversations into written requirements, timelines and delivery plans
- Shipped the platforms clients run their business on: multi-leg trip booking with vendor bidding and payment, academic publishing with article-processing charges, driver onboarding with automated identity verification, and a technician marketplace
- Designed and integrated REST APIs and webhook flows with retry and idempotency handling, keeping client applications available when third-party services failed
- Set up the project AI development workflow: custom agents, MCP servers and Claude Code skills, a written architecture spec agents must follow, and a QA review step that runs before merge
- Replaced manual customer follow-up with scheduled email and SMS workflows on n8n and LLM APIs, covering webinar reminders, deposit alerts and overdue returns
- Improved Core Web Vitals across client sites through code splitting, image optimization and caching
- Deployed and maintained applications on Linux (Ubuntu) with Docker, Nginx and PM2, including CI/CD, SSL and production incident response
- Managed deployment credentials and environment secrets across internal and client servers, controlling repository and server access across GitHub and GitLab
- Coordinated across design, backend and mobile teams, ran client feedback cycles through delivery, and mentored junior developers on the team

### Web Developer - Embassy IT Solutions (Sep 2022 - Oct 2023)
Bengaluru, India
- Delivered client web applications in React, with reusable component libraries and responsive layouts
- Integrated REST APIs and third-party services, including authentication flows and client-specific feature work
- Debugged and resolved production issues across live client sites: browser compatibility, performance regressions and API failures

### Frontend Developer - Embassy IT Solutions (Jul 2022 - Sep 2022)
Bengaluru, India
- Developed UI components and responsive layouts for client web projects
- Promoted to Web Developer after three months, taking on API integration and full project delivery

## Independent Projects
<!-- The projects below were delivered for clients, listed on the CV under Projects. -->
- **WeDrive Global ERP** (app.wedriveglobal.com; Next.js, TypeScript, Sequelize, MySQL): Authored the 44-section business-architecture spec defining the booking domain, separating a commercial layer (lead, quote, one payment) from an operational layer of N independent trip legs, with 25 named invariants. Engineered the multi-leg booking engine covering 4 service types under one quote and one payment, with per-trip pricing across 2 currencies and independent trip lifecycles. Designed the vendor RFQ and bidding flow and 5 role-scoped dashboards enforcing data isolation.
- **IJSREM Journal Platform** (ijsrem.com; Next.js, TypeScript, Sequelize, MySQL): 6-stage submission and peer-review workflow (author submission, automatic reviewer assignment, reviewer reports, accept/reject decisions, copyright handling, publication). Article-processing-charge payments with GST, transactional email, role-based access for authors, reviewers and editors, and SEO for published articles.
- **Lions Go Mobility** (React, TypeScript, Node.js, Express, MySQL, React Native): 14-screen admin portal covering fleet, drivers, KYC review, live location tracking and payments, plus REST API with JWT auth and KYC verification across 3 government ID types (Aadhaar, PAN, driving licence). React Native app shipped to Android and iOS stores, with S3 media storage, cron-driven SMS alerts and GitHub Actions staging deploys.
- **JPSCE Bookkeeping Portal** (bookkeeping.jpsconsultingengineers.com; React, TypeScript, Node.js, MySQL): JWT access/refresh rotation with silent renewal, email-OTP two-factor, five-tier role-based access control. Invoicing, backlog, timesheet and reporting modules with QuickBooks API integration, deployed to AWS through GitHub Actions.
- **FieldITXperts (TechX)** (React, TypeScript, Node.js, Express, MySQL): Technician marketplace with one unified login routing 3 roles to separate portals, OTP email signup and password reset. Public technician discovery with L1/L2/L3, location, skill set and certification filters, with contact details withheld until a company engages.
- **AdvanceAgility** (advanceagility.com; Laravel, PHP, JavaScript, MySQL): AI chatbot backed by a site-content crawler, and scheduled webinar reminder emails with admin management views.
- **WaPass Injury Patient Tracking** (React, TypeScript, Laravel, MySQL): Patient injury records with follow-up scheduling on a week-calendar view across 2 user roles, scheduled email and in-app reminders, role-based access and audit trails. OAuth 2.0 integration with eClinicalWorks using JWKS and signed assertions.

## Technical Skills

### Programming & ML
- **Languages and frameworks:** JavaScript, TypeScript, React.js, Next.js, Node.js, Express.js, HTML5, CSS3
- **Frontend:** Redux Toolkit, Context API, React Hooks, Tailwind CSS, ShadCN, Responsive Design, Core Web Vitals, Accessibility (WCAG)
- **Backend and APIs:** REST API Design, Webhooks, Authentication and Authorization, JWT, OAuth 2.0, Sequelize ORM
- **Databases:** SQL, MySQL, PostgreSQL, MongoDB, schema design, migrations and seeding
- **AI engineering:** MCP server development and integration, building AI agents, Claude Code skills, plugins and hooks, agentic QA pipelines, spec-driven AI development
- **AI integration:** LLM API integration, retrieval-augmented chatbots, n8n workflow automation, prompt engineering, Claude Code, GitHub Copilot
- **Project-level use (not listed in CV Skills):** React Native, Laravel, PHP

### Domain Expertise
- Client web application delivery for customers in the UK, US and India
- Booking, logistics and vendor marketplaces; academic publishing; KYC and driver onboarding; bookkeeping; healthcare patient tracking
- Workflow automation
- Commerce and CMS: Headless CMS, Shopify, Shopify Hydrogen, WordPress, WooCommerce

### Software & Tools
- Next.js rendering: App Router and SSR/SSG/ISR in production on IJSREM and SST USA (sstcae.com, a new project)
- API styles: REST and GraphQL (GraphQL used; project not recorded)
- Testing: Jest and Playwright for automated tests, and built a personal AI testing agent on Claude Code that works with most LLMs
- Infrastructure and DevOps: Linux (Ubuntu), Docker, Nginx, PM2, VPS administration, CI/CD, AWS, Google Cloud Platform, Vercel, Render
- Version control and access: Git, GitHub, GitLab, GitHub Actions, branching strategy, code review, repository and credential access management
- Tools: Postman, Figma, Jira, Agile delivery
- Delivery: Requirements gathering, PRDs, effort estimation, client communication, cross-team coordination, mentoring

## Publications
<!-- Articles, not peer-reviewed. Venues and dates are on the LinkedIn profile; add them here if wanted. -->
1. Reliable Webhooks: Handling Retries, Duplicates, and Failure
2. Production Deployments Fail Without a Recovery Plan
3. Next.js Parallel Routes for Complex Dashboard UIs
4. Your API Is Becoming an Interface for AI Agents

## Certifications
None yet. Candidate wants free, useful certifications - see `upskill` suggestions.

## Awards
None listed.

## References
Available upon request.
