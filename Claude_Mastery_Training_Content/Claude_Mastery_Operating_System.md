# Claude Mastery — Your Cowork Project Operating System

**Goal:** become a world-class Claude power user — fluent across every surface of the Claude ecosystem, able to build real workflows, and able to teach it. This file is the operating system for a Cowork project dedicated to that goal.

**Reality check on "most advanced user in the world":** the Claude ecosystem ships new capabilities constantly, so true mastery is not a fixed finish line — it's **depth across the whole surface + the discipline to stay current + building real things + teaching others.** This file is built to drive all four. It's documentation-verified as of June 2026; re-verify specifics against official docs (Part 6), because features change fast. **You set the pace** — work through this at whatever speed and order suit you; there are no schedules here, only a sequence and a method.

---

## 0. How to set up and use this in your Cowork project

1. **Create the Cowork project** (Claude Desktop → Cowork → new project, e.g. "Claude Mastery").
2. **Paste Part 1 into the project's instructions.** That turns every chat in this project into a coaching session aimed at your mastery.
3. **Add this file to the project's knowledge** so Claude always has the full curriculum and map on hand.
4. **Work the curriculum (Part 3)** one capability at a time, in whatever order suits you, on *real* tasks from your BJ's enablement role wherever possible — you learn fastest building things you actually need.
5. **Use the learning loop (Part 4)** for each capability, and the frontier-tracking routine (Part 5) so you stay current as the product evolves.
6. **Self-assess against the rubric (Part 7)** whenever you want a progress check.

**The mastery loop, four moves:** *Do* it on a real task → *Explain* it (could you teach a non-technical colleague?) → *Build* something with it → *Stay current* as it changes. A capability isn't "mastered" until all four are true.

---

## 1. Project instructions — paste this into your Cowork project

```
ROLE OF THIS PROJECT
This is my dedicated "Claude Mastery" project. Your job here is to make me a
world-class Claude power user — one of the most advanced users of Claude anywhere.
Act as my expert Claude tutor, coach, and sparring partner. Be rigorous, push me,
and hold a high bar.

ABOUT ME
I'm the AI Adoption & Enablement Lead at BJ's Wholesale Club. I'm building an
enterprise AI enablement program and coordinating a network of Champions who train
hundreds of employees on Claude, ChatGPT, and Microsoft 365 Copilot. So I need to
master Claude both as a power user AND well enough to teach it, build training and
accelerators with it, and brief leadership on it. Tie lessons to that context where
it helps, and use real BJ's-style tasks as practice.

HOW TO TEACH ME
- Teach by doing. For every capability, have me actually use it on a real task, not
  just read about it. Give me an exercise, watch what I produce, then critique it.
- Go deep, not just broad. Cover core, advanced, new, and lesser-known features —
  the "when and why," the edge cases, the gotchas, and how power users actually use
  each thing. Don't assume I already know something; proactively surface features I
  may be unaware of.
- Always tie a capability to (a) a real use case and (b) how I'd teach it to a
  non-technical business person, since that's my job.
- Quiz me. End sessions by checking my understanding and flagging gaps. Track what
  I've mastered and what's next against the curriculum in this project's knowledge.
- Be honest. Lead with the answer, then the nuance. Tell me when I'm doing something
  the slow or wrong way, and show me the better pattern.
- I set the pace. Don't rush me or impose a schedule; go as deep as I want on each
  topic and move on when I'm ready.

STAY CURRENT — DO NOT RELY ON MEMORY FOR FEATURE DETAILS
Claude changes constantly. Whenever we discuss a specific feature, capability, limit,
model, or price, verify it against current official documentation before teaching
it as fact, and flag anything new, recently changed, or uncertain. Authoritative
sources: support.claude.com (Claude.ai), docs.claude.com / platform.claude.com
(developer platform), code.claude.com (Claude Code), and claude.com/blog +
anthropic.com/news for announcements. When something may have changed since your
training, say so and check.

OUTPUT STYLE
Plain, confident, practical. Use real examples and step-by-step demos. When you
build something with me (a Skill, a Project setup, an artifact, an agent), produce
the actual artifact, then explain the choices so I learn the pattern.

You don't need me to re-explain any of this each time.
```

---

## 2. The territory — the complete Claude ecosystem map

You can't be a master of something you can't see the edges of. This is the full landscape to cover. Each item is expanded into objectives and exercises in Part 3.

### 2.1 The models (the engine)
- **Haiku 4.5** — fastest and cheapest; great for high-volume, simple, latency-sensitive tasks.
- **Sonnet 4.6** — the balanced everyday workhorse; the production default for most work.
- **Opus 4.8** — the most capable standard model; for the hardest reasoning, analysis, and long-context work (higher cost per token).
- **Mythos-class (Claude Mythos 5 / Fable 5)** — the frontier tier: ~1M-token context, can delegate to large numbers of parallel subagents, built for long-horizon autonomous work. Access is restricted/limited — know it exists and what it's for even if you can't use it yet.
- **Reasoning controls** — *extended thinking* (the model reasons in a scratchpad before answering) and *effort* controls. Master *when* deeper reasoning is worth the time/cost and when standard mode is better.
- **Key boundary:** Claude takes text and image input and produces text/code output — it does **not** natively generate images, audio, or video. Know this so you set expectations correctly when teaching.
- **How you customize Claude:** through prompting, system prompts, Projects, Styles, and Skills — Claude isn't customer fine-tuned, so invest your effort there rather than looking for a "train your own model" path.
- **True of every current model:** multilingual, with text + image input and text output. Model lifecycle to track: stable **model IDs & versioning**, **model cards**, a published **pricing** page, and a **deprecation policy** (older models are retired on notice) — so part of your job is always knowing which model is current.

### 2.2 Claude.ai — the chat surface (your daily cockpit)
- **Core chat** — prompting, context, iteration, formatting control.
- **Conversation branching** — edit one of your earlier messages, or use **Retry / regenerate** on a response, to fork the chat into a new branch you can compare against the original without losing it (toggle between versions). A genuine power-user move: explore alternative phrasings, and reuse a well-set-up context as a "branch point" for several related questions.
- **Prompt engineering** — beyond basic prompting: **system prompts**, **XML tags** to structure inputs and outputs, **multishot (few-shot) examples**, **chain-of-thought**, **prefilling** Claude's reply, and reusable **prompt templates** with variables. Anthropic publishes a full prompt-engineering guide, and the developer console has a **prompt generator** and **prompt improver**. This is core to both your results and teaching others.
- **Projects** — persistent workspaces with a knowledge base + custom instructions; org sharing; automatic RAG over large knowledge bases; per-project memory.
- **Artifacts** — self-contained outputs (docs, dashboards, diagrams, calculators, single-page HTML tools); can be **AI-powered** (call the Claude API at runtime) and use **persistent storage**; on Enterprise they're shared **internally only** (no public web publishing); the "Imagine"/visual side.
- **Inline visualizations** — beyond the artifacts side panel, Claude can draw interactive charts and diagrams directly inside the chat.
- **Memory** — Claude remembering context across chats; project-scoped memory; generating memory from chat history; managing what's remembered.
- **Skills** — packaged, reusable workflows (a SKILL.md folder + optional scripts/resources) that load on demand; built-in skills (Excel, PowerPoint, Word, PDF); custom and org-provisioned skills.
- **Styles** — per-chat tone/voice presets (Normal, Learning, Concise, Explanatory, Formal) plus custom styles built from a writing sample or a prompt. (Per Anthropic's docs, Styles are migrating into Skills; both surfaces work for now.)
- **Web search & Research** — live web grounding and multi-source deep research.
- **Vision** — reading screenshots, diagrams, photos, documents.
- **Files & PDF** — uploading and working with documents and data.
- **Analysis tool / code execution & file creation** — Claude running code to compute, analyze data, and create files in chat.
- **Enterprise Search** — connect internal knowledge bases and documents so Claude answers from your organization's own content.
- **Connectors / MCP in chat** — Google Workspace (Docs, Sheets, Gmail), GitHub, Slack, Microsoft 365, and more; plus anything custom via MCP.
- **Search & reference past chats** — pulling from your conversation history.
- **Voice input** — the microphone in the compose bar transcribes speech in real time (editable before sending); good for brain-dumps and brainstorming.
- **Shared chat links** — share a read-only snapshot of a conversation; in a Project on Team/Enterprise you can also post a great chat to the team activity feed.
- **Chat management** — rename, star/favorite, archive, and delete chats; organize them; and move chats into or out of Projects (which also controls what's included in project memory).
- **Citations & languages** — when Claude searches the web, runs Research, or uses connectors, it **cites its sources** in the answer; and it works across **many languages** for both input and output.

**Settings, personalization & privacy — don't skip these (they're also the first things you'll teach others to set up):**
- **The personalization stack — three layers that stack on every reply:** (1) **Profile / "Instructions for Claude"** — your account-wide custom instructions in *Settings → General → Profile* (your name, what Claude calls you, your work function, and a free-text "what should Claude consider in responses" — the global layer you set once so you stop re-explaining yourself); (2) **Project instructions** — per-project context; (3) **Styles** — per-chat tone. Master all three and *when* to reach for each.
- **Capabilities toggles** (*Settings → Capabilities*) — turn web search, code execution & file creation, Artifacts, and memory on or off. Check these so you're not silently missing features, and so you can tell others how to switch them on.
- **Long-context toggle** — for very large inputs, the extended (up to ~1M-token) context is enabled in settings on supported models.
- **Privacy & data controls** (*Settings → Privacy / data-privacy controls*) — the "Help improve Claude" training toggle and its retention implications, "Search and reference chats," pausing or clearing memory, and deleting data. Essential to understand for your responsible-use guidance.
- **Incognito mode** — a per-chat ghost icon that keeps a conversation out of your history and out of training, with memory disabled; for sensitive topics. (Worth knowing for your guidance: on Team/Enterprise, incognito chats still fall under your org's data-retention and export policies.)
- **Memory management** — review, edit, and delete what Claude remembers (ask "what do you know about me?"; tell it to forget specific details).
- **Accessibility & appearance** — light / auto / dark themes, a dyslexia-friendly font, and task-completion notifications for long runs; plus keyboard shortcuts for power users.
- **The AI Migrator** — a helper that imports your preferences (and can carry over context) when moving from another assistant — handy when you're onboarding people to Claude.

### 2.3 Claude Cowork — the agentic knowledge-work desktop (the surface this project lives in)
- An agentic desktop app for non-developers: you describe an outcome and Claude plans and executes multi-step work, producing real deliverables (docs, decks, dashboards, sent communications).
- **Folder/file access** — Claude can read, edit, and create files in a folder you grant (back up first; review changes).
- **Sub-agents** — Cowork can spin up parallel sub-agents for parallelizable work.
- **Plugins** — extend Cowork with packaged capabilities; org plugin marketplaces; you can build your own.
- **Projects in Cowork** — organize tasks into workspaces with their own files, instructions, and memory.
- **Tools in Cowork** — it can drive Claude in Chrome, Excel, PowerPoint, and Design as tools.

### 2.4 Claude Code — the agentic coding/automation tool (even non-developers benefit)
- Runs in the terminal, VS Code, JetBrains, the desktop/mobile app, and the browser; the terminal CLI and VS Code can also use third-party model providers.
- **Agentic coding** — reads a codebase, plans, edits across files, runs tests.
- **Subagents & multi-agent orchestration ("Agent Teams")** — a lead agent delegating to specialized parallel subagents.
- **Background agents** — run several full sessions in parallel and watch them from one screen (the **Agent view**).
- **Auto memory & session management** — Claude saves learnings (build commands, debugging insights) across sessions on its own; resume or fork past sessions with `--continue` / `--resume` / `--fork-session`.
- **CLAUDE.md** — a project file that gives Claude persistent context, conventions, and instructions for a codebase or folder.
- **Slash commands & custom commands**, **hooks**, **/loop**, **/effort**, **Auto mode**, **Safe mode** — automation and control of the agent loop.
- **Checkpoints / rewind** — undo agent changes; **headless / CI mode** and **GitHub Actions** integration for automation.
- **Plugins & plugin marketplaces** (loadable from .zip and URLs), **MCP servers**, **Skills**, **computer use in the CLI**.
- **Managed settings, permissions, and OS sandbox** — enterprise/IT controls.
- **Publishing artifacts** from a Code session; **/usage** attribution and spend caps.

### 2.5 The Claude apps (Claude in your tools)
- **Claude in Chrome** — a browsing agent that can navigate, click, and fill forms.
- **Claude in Excel** — a spreadsheet agent/sidebar for building, updating, and explaining workbooks.
- **Claude in PowerPoint** — a slides agent.
- **Claude Design** — a canvas + design tools you iterate on via chat; imports your design system; works with Claude Code; at claude.ai/design.
- **Claude on mobile** — chat on the go, including voice input; can reach Cowork and Code remotely.

### 2.6 The Developer Platform / API (where you go from user to builder)
- **Messages API** and the model lineup; **streaming**; **structured outputs**.
- **Tool use / function calling** — giving the model tools to call, including **built-in (server) tools**: web search, web fetch, code execution, computer use, the text-editor tool, bash, and the **advisor tool**; plus **parallel tool use**, **strict tool use**, and **tool-choice** control.
- **Tool infrastructure (at scale)** — **tool search** (discover tools dynamically), **programmatic tool calling**, **fine-grained tool streaming**, tool combinations, and managing tool context.
- **Extended thinking** via the API; **vision**; **files & PDF support**; **citations**.
- **Context management** — the **memory tool** and **context editing** (store/retrieve beyond a single context window; distinct from the app's chat memory), plus **compaction**, **mid-conversation system messages**, **orchestration mode**, **cache diagnostics**, and **token counting**.
- **Prompt caching** (cache reused context cheaply) and the **Batch API** (50% discount, async).
- **Prompt & eval tools** — the **Workbench** plus **prompt generator / improver** for building and testing prompts in the browser, and **evals / batch testing** for measuring prompt and agent quality.
- **Citations for custom RAG** — **search-result content blocks** let your own tools return sources that Claude cites automatically (matching web-search citation quality).
- **Skills API** (`/v1/skills`) — provisioning skills programmatically.
- **Agent SDK** — standard patterns for building multi-agent systems.
- **Managed Agents** (cloud-hosted): **Dreaming** (agents review past sessions and curate memory), **multiagent orchestration**, **Outcomes** (a grader rubric that sends an agent back to revise), **scheduled deployments** (cron), and **webhooks**.
- **Deployment options** — Claude via the Anthropic API and on **AWS Bedrock, Google Vertex AI, and Microsoft Foundry** (matters when IT decides where Claude runs). Note: **embeddings for RAG** come from partner models (e.g., Voyage AI), not a first-party Anthropic embeddings model.
- **Console & org tooling** — the **Developer Console** with **Workspaces** (segment projects, keys, and spend), **API keys**, the **Cost & Usage pages**, **rate limits / usage tiers**, the **Usage and Cost API**, the **Admin API**, and the **Compliance API** (compliance/eDiscovery) — the governance surface relevant to your enablement work.
- **SDKs & learning resources** — official client libraries for **Python, TypeScript, C#**, and more, plus the **Cookbook** and **Quickstarts** for worked, runnable examples.

### 2.7 MCP & connectors (the integration layer that makes Claude useful at work)
- **Model Context Protocol (MCP)** — the open standard for connecting Claude to external tools, data, and services through a common interface.
- **Remote MCP connectors**, **one-click local MCP** on Desktop, and **enterprise-managed MCP** (admins provision connectors via the identity provider, e.g. Okta, so users get zero-touch access).
- **Building & sourcing connectors** — you can **build your own MCP server** to expose internal tools and data, browse the **connectors directory**, and use **OAuth** for secure remote authorization.

### 2.8 The enterprise / admin layer (your professional edge)
IT owns these controls, but because your job is org-scale enablement they're part of *your* mastery — you need them to advise the platform team, deploy accelerators safely, guide responsible use, and brief leadership. The deep, BJ's-specific versions of cost and responsible AI live in your master plan (Sections 7 and 9); this is the map of what the Claude admin layer covers.

- **Identity & access** — SSO (SAML 2.0 / OIDC); user provisioning via SCIM (recommended), Just-in-Time, or manual; domain capture (auto-route your domain's users); role-based permissions (Primary Owner / Owner / Admin / Member); the **Admin API** for programmatic org management.
- **Cost & spend governance** — on usage-based Enterprise, the seat covers *access* and usage is billed at API rates on top, so **spend limits at org, group/seat-tier, and user level are the key control** (the default is no cap). Levers: usage credits, model right-sizing (Haiku/Sonnet vs. Opus), prompt caching, batch, and Claude Code per-session caps. *(Full version: master plan §7.)*
- **Sharing & collaboration controls** — org-wide **Skills provisioning** (Owners) plus member-to-member and org-directory Skill-sharing toggles (off by default); **project sharing** (org-wide or to named people; "Can use" / "Can edit"; admins can enable/disable public projects); **artifact** internal-only sharing; **connector restrictions** (verified-domain) and **enterprise-managed MCP** (provision connectors through your IdP, e.g. Okta, for zero-touch access); and the unified **connectors / Skills / plugins directory**.
- **Capability controls (org-wide toggles)** — set a **default model**; enable/disable **Code Execution & file creation, Skills, Cowork, web search, and public projects**; Cowork **network-egress allowlists**; and Cowork **org branding**.
- **Data protection & compliance** — no training on your data; **configurable retention**; **data residency**; **audit logs**; the **Compliance API** (real-time usage data for monitoring/eDiscovery); **OpenTelemetry** streaming to your SIEM; **SOC 2 Type 2 / ISO 27001** certifications and **HIPAA-readiness**; and clear data-ownership / processor-vs-controller terms.
- **Responsible AI & monitoring** — the enterprise data-protection model is the first guardrail; monitor via **audit logs, the Compliance API, and usage analytics**; respond fast by **blocking a specific agent, Skill, or connector**; and pair all of it with your own enablement guidance and the preventive / detective / responsive / cultural mechanism model. *(Full version: master plan §9.)*
- **Usage analytics & reporting** — the **usage analytics** dashboard and **"analytics chat"** (ask Claude about your org's usage), plus seat and spend reporting — the raw material for your adoption metrics.
- **Deployment & procurement** — Enterprise via direct contract or **AWS Marketplace**; self-serve vs. sales-assisted; and Claude available on **AWS Bedrock / Google Vertex / Microsoft Foundry** (see §2.6) when IT chooses where it runs.
- **Plan awareness** — Free / Pro / Max / Team / Enterprise, and seat types — so you can advise who needs what.

---

## 3. The mastery curriculum — leveled, with exercises and mastery checks

Work through these in whatever order and at whatever pace suit you. Each level builds on the last, so this sequence is a sensible default. For each capability, *do the exercises on real tasks*, then run the mastery check. Where it says "teach-back," actually write or record how you'd explain it to a non-technical colleague — that's the bar for your job.

### Level 1 — Foundations (the bedrock that makes everything else work)
**Learn:** prompting that works (role, task, audience, format, constraints, examples); the building blocks of **prompt engineering** (system prompts, XML tags, multishot examples, chain-of-thought, prefilling, reusable templates); giving context; iterating to refine an answer; verifying outputs; choosing the right model and when to use extended thinking; the basics of the chat surface.

**Exercises**
1. Take a weak one-line prompt and improve it through five iterations; note what each change bought you.
2. Run the same real task (e.g., "summarize this 30-page policy") on Haiku, Sonnet, and Opus; compare quality, speed, and when each is the right call.
3. Turn a messy request into a structured prompt that returns exactly the format you want (a table, a 5-bullet brief, a draft email).
4. Deliberately catch a Claude mistake by verifying a factual claim against a source.
5. Use extended thinking on a genuinely hard reasoning task and a simple one; feel the difference.
6. Build a reusable **prompt template** (with placeholders) for a task you do often, using XML tags and a worked example; run a weak prompt through the console's prompt improver and study the changes.

**Mastery check:** you reliably get a great result on the first or second try, you structure prompts with tags and examples, you choose models deliberately, you never take output as truth without checking, and you can teach prompting and basic prompt engineering in ten minutes.

### Level 2 — Power User (the features that 10x your daily work)
**Learn:** Projects (knowledge base + custom instructions + sharing); Artifacts (build and share an internal tool); Memory (and how to manage it); Styles; Web search & Research; Vision; Files/PDF; the analysis/code-execution tool; **Enterprise Search**; connectors (Google Workspace and others).

**Exercises**
1. Build a Project with a knowledge base and custom instructions for a real workstream; prove it beats re-pasting context every time.
2. Have Claude build an **artifact** — e.g., an adoption-metrics dashboard or an ROI calculator — and share it internally.
3. Run a **Research** task that needs real breadth; compare it to a single web search.
4. Drop in a screenshot/diagram and have Claude read and act on it (vision).
5. Upload a spreadsheet or dataset and have the analysis tool compute and chart something real.
6. Create a **Style** that matches BJ's associate-first voice and reuse it.
7. Connect a knowledge source (or use **Enterprise Search**) and have Claude answer from your org's own content; compare to pasting files.

**Mastery check:** you instinctively reach for Projects/Artifacts/Research/Analysis/Enterprise Search at the right moments, you can build a shareable internal tool from scratch, and you can teach each of these to a beginner with a live demo.

### Level 3 — Workflow Architect (packaging and automating real work)
**Learn:** **Skills** — what they are, how to author a SKILL.md, test it, document it, and (with the platform team) provision it org-wide; **Cowork** — running agentic multi-step tasks, using sub-agents, and plugins; the **Claude apps** (Chrome, Excel, PowerPoint, Design) as power tools.

**Exercises**
1. Author, test, and document one **Skill** that encodes a repeatable BJ's workflow (e.g., a standard report format or a brand-voice rewriter). Then plan how you'd provision it to the org.
2. Give Cowork a real multi-step deliverable (e.g., "analyze this folder of feedback and produce a summary deck") and watch it plan, use sub-agents, and produce files — review every change.
3. Use Claude in Excel on a real workbook and Claude in PowerPoint to build a deck; note where each shines.
4. Build something in Claude Design from a prompt and iterate on the canvas.

**Mastery check:** you can package a workflow as a Skill end-to-end, you can hand Cowork a genuinely complex task and supervise it well, and you can demo the apps convincingly to a skeptical team.

### Level 4 — Agentic & Developer (cross the line from user to builder)
**Learn:** **Claude Code** (even if you're not a developer — agentic automation, subagents/Agent Teams, CLAUDE.md, slash/custom commands, headless mode, hooks, plugins, MCP, computer use); **MCP** (connect Claude to a tool/data source); the **API / Developer Platform** (tool use including built-in tools, prompt caching, batch, files, structured outputs, the memory tool/context editing); **evals**; the **Agent SDK** and **Managed Agents** (Dreaming, orchestration, Outcomes, scheduled deployments, webhooks); and deployment options (API vs. Bedrock/Vertex/Foundry).

**Exercises**
1. Install Claude Code and have it do something real (e.g., reorganize a folder of training files, or build a small internal script/tool); try a subagent task, a CLAUDE.md, and the /effort and Auto/Safe modes.
2. Connect one **MCP** server/connector and use it from chat or Code; understand the auth and least-privilege model.
3. Make a handful of API calls (even via a simple notebook): a basic message, a tool-use call, and a prompt-caching example; feel how the platform differs from the app.
4. Read how **Managed Agents** work (scheduled deployments, Outcomes, Dreaming) and design — on paper — an agent that would help your enablement program (e.g., a recurring adoption-digest agent).
5. Write a small **eval**: define a few test cases and a simple rubric for a prompt or agent, and use it to compare two prompt versions (this mirrors how the console evals and Managed-Agent "Outcomes" work).

**Mastery check:** you can wire Claude into an external tool via MCP, run Claude Code for non-trivial automation, test a prompt/agent with an eval, and explain — accurately — what the API and agent platform make possible (and their cost/governance implications), including where Claude runs (API vs. Bedrock/Vertex/Foundry), to a technical Champion or the platform team.

### Level 5 — Frontier / World-Class (depth, scale, and leadership)
**Learn:** org-scale deployment and the enterprise/admin layer (SSO/SCIM, audit, Compliance API, org Skills provisioning, usage analytics, spend governance); designing accelerators (Skills, Projects, agents) for hundreds of users; teaching and certifying others; contributing to the ecosystem (Skills directory, MCP servers, prompt patterns); and the meta-skill of **staying ahead** (Part 5).

**Exercises**
1. Design BJ's "golden path": which surfaces and accelerators each role should use, and the org-provisioned Skills/Projects/agents that support them.
2. Build a Champion-ready teaching module for one advanced capability (deck + live demo + exercise + check) — this proves mastery by forcing teach-back.
3. Write a one-page "what changed recently in Claude and what it means for us" brief — and keep doing it on your own cadence.
4. Pick one frontier capability (e.g., Managed Agents or multi-agent orchestration) and go genuinely deep until you could advise the platform team on it.

**Mastery check:** people inside BJ's treat you as *the* Claude authority; you can deploy, govern, and teach Claude at org scale; and you have a running system that keeps you current as the product evolves.

---

## 4. How to work each capability — the learning loop

Pace is yours. What matters is *how* you work each capability, not how fast. For every item in the curriculum, run this loop:

- **Do it on a real task.** Reps on actual work beat reading. Use the surface or feature on something you genuinely need.
- **Build something with it.** Produce a real artifact — a Skill, a Project, an agent, a deck, a tool. Building is what cements a capability.
- **Teach it.** Draft how you'd explain it to a non-technical Champion: the one-liner, the live demo, the "first try this." If you can't teach it cleanly, you haven't mastered it yet.
- **Review and quiz.** Have your tutor (this project) check your understanding, surface gaps, and update your rubric.

**Depth over breadth.** Fully absorb one capability — including its edge cases and gotchas — before moving to the next. One capability truly mastered is worth more than ten skimmed. Move on when the mastery check for that item is genuinely true, not before — and take as long as that needs.

---

## 5. Staying at the frontier (how to be — and stay — one of the most advanced users)

Being "the most advanced" is less about knowing everything today and more about a system that keeps you ahead as Claude ships new capabilities. Run this on whatever cadence suits you:

- **Monitor the official channels.** Claude Code updates, the Claude.ai "what's new," the developer platform changelog, claude.com/blog, and anthropic.com/news. A quick skim of the release notes is enough to never be blindsided.
- **Triage every new feature.** For each release ask: *What is it? Who is it for? Does it change how I (or my Champions, or BJ's) should work?* Most releases are "noted." A few are "adopt now." Keep a running log of the few that matter.
- **Adopt deliberately, one at a time.** Don't chase every update. Test a new capability against a real workflow; keep it only if it earns its place. That selectivity *is* expertise.
- **Engage with the ecosystem.** Explore the Skills directory and partner skills, try community/partner MCP servers, and study how power users build agents and workflows. The frontier is partly built by the community around MCP, Skills, and Cowork/Code.
- **Keep the verification discipline.** Never teach a feature, limit, or price from memory — confirm it in the current docs first. Being trusted *and* current is what makes you the authority.
- **Build in public, internally.** Share what you learn in your AI Hub, Teams channel, and Champion forum. Teaching at the frontier is how you both cement mastery and become known as the person who has it.

---

## 6. Authoritative sources (verify here — features change fast)

- **Claude.ai (app) features & how-to:** support.claude.com
- **Developer platform / API:** docs.claude.com and platform.claude.com (incl. the API changelog)
- **Claude Code:** code.claude.com / the Claude Code docs and update notes
- **Announcements & deep dives:** claude.com/blog and anthropic.com/news
- **Skills, MCP, and agents:** the Agent Skills docs, the Model Context Protocol docs, and the Managed Agents / Agent SDK docs on the developer platform
- **Learning by example:** the Anthropic Cookbook and the platform Quickstarts are excellent for hands-on patterns (prompting, tool use, agents, RAG)

Treat every model name, price, limit, and feature detail as perishable. When in doubt, check the source above and note the date you verified it.

---

## 7. Mastery self-assessment rubric

Score yourself 1–4 on each (1 = new to it, 2 = can do it with help, 3 = fluent and independent, 4 = can teach it and handle edge cases). Re-score whenever you want a progress check; your aim is mostly 3s and 4s across the board, with 4s on the surfaces your role depends on.

**Foundations**
- [ ] Prompting fundamentals (role/task/format/examples/iteration)
- [ ] Prompt engineering (system prompts, XML tags, multishot, prefill, templates)
- [ ] Context & verification habits
- [ ] Model selection + when to use extended thinking

**Power user**
- [ ] Projects (knowledge base, instructions, sharing)
- [ ] Artifacts (build + share an internal tool; AI-powered + storage)
- [ ] Memory, Styles, Files/Vision
- [ ] Web search & Research
- [ ] Analysis / code-execution tool
- [ ] Enterprise Search & connectors (Google Workspace, etc.)
- [ ] Personalization stack (global Profile, Project instructions, Styles)
- [ ] Settings & privacy (capabilities toggles, incognito, data controls, memory management)

**Workflow architect**
- [ ] Skills (author, test, document, plan org provisioning)
- [ ] Cowork (multi-step tasks, sub-agents, plugins)
- [ ] Claude apps (Chrome, Excel, PowerPoint, Design)

**Agentic & developer**
- [ ] Claude Code (agentic automation, subagents, CLAUDE.md, commands, headless)
- [ ] MCP (connect a tool/data source; auth & least privilege)
- [ ] API / platform (tool use incl. built-in tools, prompt caching, batch, structured outputs)
- [ ] Memory tool & context editing
- [ ] Evals / testing
- [ ] Agent SDK & Managed Agents (orchestration, Outcomes, scheduled, Dreaming)
- [ ] Deployment options — awareness (API vs. Bedrock / Vertex / Foundry)

**Frontier / leadership**
- [ ] Enterprise/admin layer (identity, spend governance, sharing controls, capability toggles, data/compliance, responsible-AI monitoring, analytics)
- [ ] Designing org-scale accelerators (Skills/Projects/agents for many users)
- [ ] Teaching & certifying others
- [ ] A running system for staying current (Part 5)

---

## 8. Coverage & verification (so you can check this, not just trust it)

This map exists because "have you covered everything?" should be verifiable, not a promise. Each area below was checked against the official source listed, on **26 June 2026**. To re-verify any area yourself, open the source and compare — and because the product changes, treat anything here as current *as of that date*, not forever.

| Area | Checked against |
|---|---|
| Models, IDs, versioning, deprecation | platform.claude.com/docs → Models overview, Model deprecations, Pricing |
| Claude.ai chat surface (Projects, Artifacts, Memory, Skills, Styles, search, personalization, privacy, incognito) | support.claude.com → Projects, Personalization, Chat search & memory, Privacy/data-controls articles |
| Conversation branching, regenerate, inline visualizations | support.claude.com + Anthropic news/blog |
| Cowork | Anthropic news/blog + support.claude.com |
| Claude Code (CLAUDE.md, subagents, background agents, hooks, sessions, plugins) | code.claude.com/docs → Overview and feature pages |
| Claude apps (Chrome, Excel, PowerPoint, Design, mobile) | claude.com/blog + Anthropic news |
| Developer Platform / API (tools, context mgmt, evals, Workbench, SDKs, Console, Managed Agents) | platform.claude.com/docs → Build with Claude (Features overview), Tools, Context management, Release notes |
| MCP & connectors | Model Context Protocol docs + Anthropic news (enterprise-managed MCP) |
| Enterprise / admin layer (identity, cost, sharing, compliance, analytics) | support.claude.com Enterprise articles + platform.claude.com Admin/Usage-and-Cost/Compliance API |

**Two honest limits, stated plainly:**
- A few areas are intentionally **"known but thin"** because the details aren't fully public (enterprise admin internals; the Mythos/Fable frontier tier, which is access-restricted under Project Glasswing). Those are flagged in the text rather than padded.
- Completeness is a **dated snapshot plus a habit.** New features ship continually; Part 5 is the routine that keeps this current, and the standing rule in Part 1 is to re-verify specifics against these sources before treating them as fact.

---

*Built June 2026 and documentation-verified as of that date. Claude evolves frequently — re-verify specifics against the official sources in Part 6. This is a personal working reference, not an official BJ's Wholesale Club or Anthropic publication.*
