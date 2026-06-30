# Ondřej Chrastina — Full Profile
*Last updated: 2026-06-30 (deep crawl via researcher)*

## Identity
- **Location:** Brno, Czech Republic
- **Current role:** Developer Advocate at CKEditor (since ~Jul 2025)
- **Email:** ondrej@ckeditor.com / ondrej@chrastina.dev
- **GitHub:** Simply007 (220 repos, 762 contributions/year) | orgs: @ckeditor, @notum-cz, @prochrastinate
- **X:** @ChrastinaOndrej | **LinkedIn:** ondrejchrastina | **dev.to:** simply007
- **Bluesky:** simply007-cz.bsky.social | **YouTube:** @Simply007-cz
- **Self-description:** "Typo master seeking sport-beer balance. Open source lover with QA, web dev, data quality, and CMS background, practicing developer relations."

## Career Timeline
- **Early:** QA Engineer at Kentico (.NET DXP)
- **~2018–2022:** First Developer Advocate → DevRel Lead at Kentico/Kontent.ai (TypeScript/JS/.NET SDKs, headless CMS)
- **~2022–2024:** Head of Developer Relations at Ataccama (data quality, Python SDK, Snowflake/Databricks/Airflow)
- **2025–present:** Developer Advocate at CKEditor (rich-text editing, AI-assisted authoring, MCP)

## Technical Expertise
**Languages:** TypeScript/JS (primary, SDK-grade) → C#/.NET (strong) → Python → Java/Kotlin → GraphQL, SQL

**Frameworks:** React, Next.js, Gatsby, Nuxt, Astro, Svelte/Sapper, Vue, Express, Apollo

**CMS/DXP:** CKEditor 5 (current expert), Kontent.ai (deep), Kentico, Drupal, Strapi, TYPO3

**Infra:** Docker, Kubernetes, GitHub Actions, Azure, Vercel, Netlify

**Data:** Snowflake, Databricks, Airflow, DBT

**AI/LLM:** Claude/Anthropic (primary), CKEditor AI, on-premises LLM + MCP tools, autonomous agents (NanoClaw), LLM-as-judge testing

**Testing philosophy:** Integration Matrix over unit-test maximalism; canary browser lanes (caught Chrome bug 3 weeks early); LLM-as-judge for AI output quality

## Writing
**Style:** Short, actionable, practitioner-first. "A couple of minutes to read, you learn something new."

**Personal journal (10 posts, 2020–2025):** CKEditor pitfalls, custom elements, Kubernetes with AI tooling, Kontent.ai internals, Jamstack/.NET, JS async patterns

**dev.to (7 articles):** Jamstack/.NET (most popular), Kontent.ai tutorials, DrupalCon recap (vibe-coding Drupal module with Claude Code), CKEditor AI

**CKEditor blog (7 articles, Jul 2025–Feb 2026):** OAuth + real-time collab, Tiptap migration, Vue WYSIWYG comparison, AI prompt templates, AI-assisted dev use cases

## Speaking (21+ talks, 2019–2026)
**2026 highlights:**
- "The Real Story Behind AI in Content Editing" — CMS Summit Frankfurt, May 2026
- "Sleep Better on Release Day: Testing Strategy for JS SDKs" — DEVWorld Amsterdam, May 2026 (5,000 attendees)
- "Drupal in the Age of AI" — Acquia Engage Denver, Apr 2026 (dinner with Dries Buytaert)
- "Extreme TypeScript: Mastering Recursion via Type-Level Arithmetic" — Brno meetup, Apr 2026
- "CKEditor AI on Your Premises: Hook your LLM and register MCP tools" — Apr 2026
- "CKEditor in Drupal + AI-Powered Authoring" — DrupalCon Chicago, Mar 2026
- Tech Talks Daily podcast (51K monthly listeners), Hackmamba, Bas.fm, AI Master Podcast

## Key Opinions
**On AI:**
- "Stop chatting, start delegating" — agents over chatbots
- "A ChatGPT license is not a content strategy" — recurring theme
- BYOAI problem: 78% of workers use personal AI → compliance + inconsistency → embedded AI thesis
- SKILL.md + PROMPT.md pattern for repeatable Claude Code workflows
- LLM provider swap should be a first-class design requirement

**On DevRel:**
- In the AI era: shift from "how to" → "why this"
- Friction reduction is core; eliminate unnecessary setup complexity
- Short, actionable > long docs

**On TypeScript:** Advanced type-level programming is worth it; type system is Turing-complete

**On testing:** Integration Matrix > unit-test maximalism; canary lanes catch real-world regressions

## Notable Projects
| Project | What |
|---|---|
| ts-type-arithmetic | Compile-time calculator in TS type system — educational |
| kontent-template-gatsby-landing-page-photon | JAMstack template; in official Gatsby gallery (12★) |
| kontent-environments-comparer | Vue tool to diff two Kontent.ai environments |
| proactive-digital-twin-workshop | NanoClaw workshop kit (47 commits Jun 2026) |
| upcloud-doom | Classic DOOM on Kubernetes, browser-streamed via noVNC |
| volby2025 | Real-time Czech Parliament election monitor |
| Official Next.js example for Kontent.ai | Contributed to Next.js official examples |

## Workshop: Proactive Digital Twin (Current Focus)
**Event:** Web Summer Camp 2026, Opatija, Croatia — **July 2, 2026** (AI Engineering track)
**Repo:** https://github.com/Simply007/proactive-digital-twin-workshop
**Duration:** 2h 30min | Audience: intermediate web devs

**Core thesis:** Proactive vs. reactive AI is a deployment shape difference, not a model quality difference.

**"Living Files" philosophy:** Agent behavior encoded in Markdown (CLAUDE.local.md, CLAUDE.md) — human-readable, version-controllable. "This is just text. The agent reads it every time it wakes up. That's the whole trick."

**Stack:** NanoClaw + Claude Sonnet 4.5 + Ubuntu 26.04 VM + Telegram + GitHub private repo (memory sync) + OneCLI (natural language → cron)

**4 exercises:**
1. Deploy NanoClaw + Telegram, ping/pong (40min)
2. Agent interviews user → writes CLAUDE.local.md (15min)
3. GitHub OAuth → memory sync → hourly schedule (25min)
4. Community-voted use case + proactive notification (20min)

**Hosting tested:** Workshop day on local VM (free); post-workshop: Hetzner CAX11 (~€4.51/mo) recommended
