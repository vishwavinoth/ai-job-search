---
framework_version: 1.0.0
---

# Interview Preparation Guide

<!-- SETUP: STAR examples are personalized by running /setup based on your actual experience -->

## STAR Format

Structure answers as: **Situation** (context), **Task** (your responsibility), **Action** (what you did), **Result** (outcome).

Keep answers to 1-2 minutes. Be specific. End with what you learned or would do differently.

## Ready-Made STAR Examples

<!-- Drafted from the CV. Each Result needs your real outcome before you use it: nothing here was invented, so results without a number on the CV are marked TO ADD. -->

### 1. WeDrive Global ERP (System design and domain modelling)
**S:** A client needed one booking to cover several service types and independent trip legs, under one quote and one payment.
**T:** Define the domain and build the booking engine so later changes would not break it.
**A:** Wrote a 44-section business-architecture spec separating the commercial layer (lead, quote, payment) from an operational layer of N trip legs, with 25 named invariants. Built the engine for 4 service types with per-trip pricing across 2 currencies, plus vendor RFQ and bidding and 5 role-scoped dashboards.
**R:** Live at app.wedriveglobal.com. TO ADD: usage or business outcome.
**Use for:** "Tell me about a complex system you designed", "How do you handle ambiguous requirements?"

### 2. Project AI development workflow (AI engineering and initiative)
**S:** Project development needed a repeatable way to use AI tools without losing quality.
**T:** Set up the AI development workflow for the project.
**A:** Built custom agents, MCP servers and Claude Code skills, wrote an architecture spec agents must follow, and added a QA review step that runs before merge.
**R:** TO ADD: effect on delivery speed or defects.
**Use for:** "How do you use AI in your work?", "Tell me about a time you improved how a team works"

### 3. Webhook reliability (Debugging and production reliability)
**S:** Client applications depended on third-party services that could fail.
**T:** Keep the applications available when those services failed.
**A:** Designed REST API and webhook flows with retry and idempotency handling.
**R:** Client applications stayed available during third-party failures. TO ADD: a specific incident.
**Use for:** "Tell me about a production issue", "How do you design for failure?"

### 4. Customer follow-up automation (Workflow automation)
**S:** Customer follow-up was manual.
**T:** Replace it with something that ran without staff effort.
**A:** Built scheduled email and SMS workflows on n8n and LLM APIs for webinar reminders, deposit alerts and overdue returns.
**R:** Manual follow-up replaced. TO ADD: hours saved or response rates.
**Use for:** "Tell me about something you automated", "How do you find business value in technical work?"

### 5. End-to-end delivery with sales and client teams (Ownership and communication)
**S:** Client projects started as sales conversations rather than specifications.
**T:** Turn them into plans the team could deliver.
**A:** Worked with sales on scoping, wrote requirements, timelines and PRDs, coordinated design, backend and mobile teams, and ran client feedback cycles.
**R:** TO ADD: a project delivered and how it was received.
**Use for:** "Tell me about working with non-technical stakeholders", "How do you manage conflicting priorities?"

## Common Tough Questions

### "Why did you leave [previous company]?"
> Draft: "I've grown a lot at Nexevo owning projects end to end. I'm now looking for a role with a bigger technical challenge and more room to grow, particularly in AI engineering." Honest and forward-looking, with no negativity about the employer.

### "You don't have [specific skill/experience]."
> Acknowledge the gap, then bridge from adjacent work: you picked up React Native, Laravel and agent tooling on delivery projects. Name how you would close it.

### "Where do you see yourself in 5 years?"
> Draft: "Building AI-driven products hands-on, with more say over architecture." Align it to the role's growth path.

### "What's your biggest weakness?"
> TO ADD: choose a genuine one with a concrete mitigation. Your own answer is needed here.

### "Do you need visa sponsorship?"
> Be direct: yes for roles outside India. Then move to what you bring and how quickly you could start.

### "Why this company specifically?"
> Customize per company. Must reference: specific projects, company values, market position, or team structure. Never give a generic answer.

## Questions You Should Ask Interviewers

### About the Role
- "What does a typical week look like in this role?"
- "What would success look like in the first 6 months?"
- "What's the biggest challenge the team is facing right now?"

### About the Team
- "How big is the team, and how do you divide work?"
- "What does the development/project lifecycle look like, from idea to production?"
- "How do you onboard new team members?"

### About Tech & Growth
- "What's your current tech stack for [relevant area]?"
- "Is there room to grow into more architectural or strategic decisions?"
- "How does the team stay current with new tools and methods?"

### About Culture (use these to prevent disappointment)
- "How would you describe the team culture?"
- "What does professional development look like here?"
- "Is there flexibility for remote/hybrid work?"
- "What's the balance between development/new projects and maintenance work?"
- "How would you describe the leadership style in this team?"
- "What do people who thrive here have in common?"

## Phone/Video Interview Tips
- Have STAR examples written out (use this file)
- Keep a glass of water nearby
- Smile when speaking (it changes your tone)
- Ask for clarification if a question is vague
- It's OK to take 5 seconds to think before answering
- End with: "Is there anything else you'd like to know about my background?"

## After the Application (Best Practice)

### Follow-Up Etiquette
- **Don't call to "stand out"** or to learn more about the role post-submission - this risks a negative impression
- If the employer specified a timeline, respect it and wait
- If no timeline was given and significant time has passed (2+ weeks), a brief call to ask about status is acceptable
- If you have genuinely new, relevant information to share, a short follow-up is fine

### Thank-You Notes
- When you receive any update (interview invitation, rejection, or status update), send a brief thank-you message
- Express appreciation for their time and the process
- Keep it short (2-3 sentences)

## Roleplay Guidelines
When the user asks for interview practice:
1. Ask which role/company to simulate
2. Start with easy warm-up questions ("Tell me about yourself")
3. Progress to role-specific technical questions
4. Include 1-2 behavioral questions using the competencies from the job posting
5. End with a tough question or curveball
6. After each answer, give brief feedback: what worked, what to sharpen
7. Suggest which STAR example would work best for each question
