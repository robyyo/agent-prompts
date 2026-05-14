# Agent Prompts Library

**Maintained by Robert Finkley** · [robertfinkley.com](https://robertfinkley.com) · [rfcgrp.com](https://rfcgrp.com)

> A curated, living library of AI prompts organized by role and use case — built for web developers, business owners, consultants, educators, and content creators who want outputs that are actually good.

---

## How to Use This Library

Each category folder contains prompt files (`.md`) with:
- **Purpose** — what the prompt does
- **Variables** — fields to customize for your context (wrapped in `{{ }}`)
- **The Prompt** — ready to copy/paste or adapt
- **Example Output** — what good output looks like

Prompts are designed to be **dynamic** — swap the variables, change the context, get a different result without rewriting from scratch.

---

## Categories

### 1. [Business](./business/)
Prompts for running and growing a business — client-facing communications, strategy, and operations.

| Subcategory | Description |
|---|---|
| [Sales](./business/sales/) | Prospecting, proposals, follow-ups, objection handling |
| [Marketing](./business/marketing/) | Campaigns, messaging, positioning, launch plans |
| [Legal](./business/legal/) | Contract summaries, policy drafts, terms and conditions |
| [Finance](./business/finance/) | Budget narratives, financial summaries, invoice templates |
| [HR & Hiring](./business/hr/) | Job descriptions, onboarding plans, performance reviews |
| [Client Communications](./business/client-comms/) | Discovery calls, status updates, difficult conversations |

---

### 2. [Productivity & Workflows](./productivity/)
Prompts for building systems that save time and eliminate busywork.

| Subcategory | Description |
|---|---|
| [Email Management](./productivity/email/) | Inbox triage, response drafts, automated filters |
| [SharePoint & M365](./productivity/sharepoint/) | List design, page templates, automation flows |
| [Project Management](./productivity/project-management/) | Task breakdowns, timelines, status reports |
| [Meeting & Documentation](./productivity/meetings/) | Agendas, action item extraction, meeting summaries |
| [CRM & Lead Tracking](./productivity/crm/) | Pipeline stages, contact notes, follow-up sequences |
| [SOPs & Process Docs](./productivity/sops/) | Standard operating procedures, workflow documentation |

---

### 3. [Design](./design/)
Prompts for creating visual and written content that looks and reads like a professional made it.

| Subcategory | Description |
|---|---|
| [Frontend UI/UX](./design/frontend/) | Web UI design systems, component aesthetics, page layouts |
| [Branding](./design/branding/) | Brand identity, voice, logo briefs, style guides |
| [Blog & Long-form](./design/blog/) | Article structures, headlines, SEO-optimized drafts |
| [Social Media](./design/social-media/) | Platform-specific posts, captions, content calendars |
| [Visual Arts & Graphics](./design/visual-arts/) | Midjourney/DALL-E prompts, illustration briefs, icon sets |
| [Presentation Design](./design/presentations/) | Slide decks, pitch decks, keynote outlines |

---

### 4. [Web Development](./web-dev/)
Prompts for writing better code, faster — from architecture decisions to debugging.

| Subcategory | Description |
|---|---|
| [Frontend Architecture](./web-dev/frontend/) | Component design, design systems, performance patterns |
| [Backend & APIs](./web-dev/backend/) | API design, endpoint specs, database schemas |
| [Code Review](./web-dev/code-review/) | Review checklists, refactor suggestions, security audits |
| [Debugging](./web-dev/debugging/) | Error analysis, root cause isolation, fix strategies |
| [Documentation](./web-dev/docs/) | README generation, inline docs, API docs |
| [Testing](./web-dev/testing/) | Test plans, unit/integration test generation |

---

### 5. [AI & Automation](./ai-automation/)
Prompts for building AI-powered systems, automations, and workflows.

| Subcategory | Description |
|---|---|
| [Prompt Engineering](./ai-automation/prompt-engineering/) | System prompts, chain-of-thought, structured outputs |
| [Workflow Automation](./ai-automation/workflows/) | n8n, Power Automate, Zapier, Make flow design |
| [AI Agent Design](./ai-automation/agents/) | Agent architectures, tool definitions, personas |
| [Chatbot & Assistant](./ai-automation/chatbots/) | Conversational flows, tone calibration, fallback handling |
| [Data Processing](./ai-automation/data/) | Extraction, transformation, classification, summarization |

---

### 6. [Education & Training](./education/)
Prompts for teaching, explaining, and building learning experiences.

| Subcategory | Description |
|---|---|
| [Course & Curriculum](./education/curriculum/) | Course outlines, module design, learning objectives |
| [Explainer Content](./education/explainers/) | Simplified explanations, analogies, concept breakdowns |
| [Tutorials & Walkthroughs](./education/tutorials/) | Step-by-step guides, how-tos, screencasts scripts |
| [Assessments & Quizzes](./education/assessments/) | Quiz generation, rubrics, knowledge checks |
| [AI Literacy](./education/ai-literacy/) | Teaching AI concepts to non-technical audiences |

---

### 7. [Content Creation](./content/)
Prompts for producing high-quality content at scale without losing your voice.

| Subcategory | Description |
|---|---|
| [Blog Writing](./content/blog/) | Research, outlines, drafts, optimization |
| [Video & Podcast Scripts](./content/video-scripts/) | Scripts, talking points, intros/outros |
| [Newsletters](./content/newsletters/) | Email sequences, weekly digests, nurture campaigns |
| [SEO & Search Content](./content/seo/) | Keyword briefs, meta descriptions, content clusters |
| [Thought Leadership](./content/thought-leadership/) | Opinion pieces, LinkedIn articles, speaker proposals |

---

### 8. [Consulting & Client Work](./consulting/)
Prompts for RF Consulting Group — discovery, delivery, and client success.

| Subcategory | Description |
|---|---|
| [Discovery & Scoping](./consulting/discovery/) | Discovery call frameworks, needs assessments, intake forms |
| [Proposals & SOW](./consulting/proposals/) | Statement of work templates, pricing narratives, scope docs |
| [Client Onboarding](./consulting/onboarding/) | Welcome sequences, kickoff agendas, expectation setting |
| [ROI & Impact](./consulting/roi/) | Value framing, before/after analysis, case study drafts |
| [Workflow Design](./consulting/workflow-design/) | Process mapping, automation audits, improvement plans |

---

## Prompt Design Principles

These prompts are built around a few core beliefs:

1. **Dynamic over static** — every prompt uses `{{ variables }}` so you can adapt it without rewriting
2. **Context-aware** — prompts ask for client/audience context upfront to avoid generic outputs
3. **Anti-slop by default** — prompts include explicit anti-genericness instructions where relevant
4. **Opinionated** — prompts make strong choices and explain why; you can push back on specifics
5. **Role-aware** — prompts are written knowing you wear multiple hats (developer, consultant, educator)

---

## Contributing & Maintaining

This is a personal living document. To add a new prompt:

1. Create a `.md` file in the appropriate category subfolder
2. Follow the template in [`_template.md`](./_template.md)
3. Add a row to the relevant category table in this README
4. Commit with a descriptive message: `add: [category] prompt for [use case]`

---

## Prompt Template

See [`_template.md`](./_template.md) for the standard prompt format used across this library.

---

*Last updated: May 2026 · Built by Robert Finkley*
