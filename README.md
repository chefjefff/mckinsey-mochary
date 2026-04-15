# 🧭 mckinsey

## Think / Plan / Operate

### A foundational operating system for AI-assisted work

*Drop-in rigor for Claude Code, Cursor, and any agentic workflow. Inspired by McKinsey's Bulletproof Problem Solving + Matt Mochary's operating system. Shareable. Portable. Free.*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude_Code-skills-orange)](https://claude.ai/code)
[![Cursor](https://img.shields.io/badge/Cursor-compatible-blue)](https://cursor.sh)

**📦 Three Claude Code skills that force McKinsey-grade rigor on every AI output.**

```bash
git clone https://github.com/chefjefff/mckinsey.git
cp -r mckinsey/skills/* ~/.claude/skills/
# Paste mckinsey/CLAUDE.md into your project's CLAUDE.md
# Done. Your AI agents now default to the triad.
```

[Jump to install →](#how-to-install-this-in-your-organization) &nbsp;·&nbsp; [Read the manifesto ↓](#the-problem) &nbsp;·&nbsp; [See the case study →](./examples/case-study-event-plan.md)

---

## The problem

You're using AI agents. They generate plans, reviews, briefs, and strategies 10x faster than you used to. Your output looks professional. But something is off.

The plans are logistics checklists ("book venue, send invites, print cards"). The reviews are retrospectives without foresight. The briefs state goals but no hypotheses. The strategies have targets but no projections. The outputs look like work — but few of them actually drive work.

This isn't a model problem. It's not a prompt problem. It's a **thinking problem**. You're getting beautifully-formatted answers to poorly-framed questions.

## The insight

Most work fails at one of three layers:

1. **Thinking** — you never properly defined the problem, cleaved it into parts, or challenged your own assumptions
2. **Planning** — you have a list of activities but no testable hypothesis, no knock-out analysis, no named owners, no funnel math
3. **Operating** — you have tasks but no single Directly Responsible Individual, no decision framework, no emotional regulation on priorities

The best problem-solvers — McKinsey partners, seasoned founders, top product operators — don't fail at these layers because they've internalized three distinct disciplines. One for each layer.

These disciplines are public knowledge. Charles Conn and Robert McLean codified the analytical one in *Bulletproof Problem Solving* (the McKinsey 7-step method). Matt Mochary codified the operating one in *The Great CEO Within* and his open-source Mochary Method curriculum. Together they form...

---

## The Triad

| Skill | Role | Source |
|-------|------|--------|
| **`/problem-solving`** | How we **THINK** | Conn & McLean, *Bulletproof Problem Solving* |
| **`/work-plan`** | How we **PLAN** | Step 4 of /problem-solving, extracted as standalone |
| **`/mochary-method`** | How we **OPERATE** | Matt Mochary, *The Great CEO Within* |

Together: analytical rigor + execution discipline + operating excellence.

### `/problem-solving` — How we THINK

*7 steps. Applies to any complex question.*

1. **Define** the problem (SMART+, problem worksheet, iterate via "porpoising")
2. **Disaggregate** with MECE logic trees (component, deductive, inductive, hypothesis, decision, ROIC)
3. **Prioritize** via 2x2 impact × ability-to-move matrix
4. **Workplan** (hands off to `/work-plan`)
5. **Analyze** heuristics first (Occam, 80:20, Rule of 72, expected value, 5 Whys) → big guns if needed (regression, Bayesian, ML, game theory)
6. **Synthesize** with the pyramid principle, visualize findings, surface cross-cutting insights
7. **Tell the story** via SCR (Situation / Complication / Resolution), storyboard with horizontal logic

**Cleaving frames** to try: ROIC, price/volume, principal/agent, assets/options, supply/demand, regulate/incent, incidence/severity, near-term/long-term.

**Bias-fighting**: obligation to dissent, multiple trees, "what would you have to believe?", pre-mortem, distributed voting, perspective-taking.

**Use when:** any complex question, strategic diagnosis, "should we do X?" decision, root-cause analysis, uncertainty management.

### `/work-plan` — How we PLAN

*Every plan, projection, or strategic output must carry these 8 elements:*

1. **Hypothesis** — "If we do X, we get Y because Z"
2. **Knock-out analysis** — the one check that kills the project if it fails. Sequence it FIRST.
3. **SCR one-day answer** — Situation / Complication / Resolution (elevator-test ready)
4. **Funnel or projection** with explicit conversion math (not just targets)
5. **6-column workplan** — Issue / Hypothesis / Analysis / Owner / Output / Due (date + time)
6. **Kill list** — what we're explicitly NOT doing, and why
7. **Risk register** — likelihood × impact × mitigation
8. **Pre-launch checklist** before locking

**Use when:** event plans, weekly priorities, proposals, campaign strategy, monthly reviews, content batches, outreach sequences, roadmap memos, sprint plans — anytime you're converting "what to do" into "who does what by when, with what expected output."

### `/mochary-method` — How we OPERATE

*Operating disciplines that surround the analytical/planning work.*

**Personal productivity:**
- **Top Goal** — 2 uninterrupted hours/day on the single highest priority, calendar-blocked, inviolable
- **Zone of Genius** — spend time only on what only you can do; delegate/kill the rest
- **Energy Audit** — color-code the calendar to spot drains

**Emotional regulation:**
- **Fear & Anger** — name it, feel it, let it go. Don't operate from a fear/anger state.

**Team operations:**
- **DRI** — every task, deliverable, decision has ONE Directly Responsible Individual
- **Agreement Tracker** — every commitment logged with owner + due date
- **Meetings** — agenda, DRI, follow-ups. No agenda = no meeting.

**Decision-making:**
- **RAPID** — Recommend, Agree, Perform, Input, Decide. Clarity on decision roles.
- **Issue / Proposed Solution** — state facts, story, proposed action with DRI + due. Never bring an issue without a proposed solution.
- **Clean Escalation** — facts + options + tradeoffs, not advocacy. Let the decider decide.

**Feedback:**
- "I noticed X → I felt Y → I'd love Z"

**Use when:** every decision, meeting, priority call, feedback moment, escalation, or emotional reaction pushing a call.

---

## The 3-question test

Before handing over any output, ask three questions:

1. **Thinking:** Is the analytical structure clear? Problem defined, tree MECE, hypotheses testable, synthesis visible? → `/problem-solving`
2. **Planning:** Does every activity tie back to a measurable outcome with a named owner and a date + time? → `/work-plan`
3. **Operating:** Is there a clear DRI for every action? Is every issue paired with a proposed solution? Is the framing facts-not-advocacy? → `/mochary-method`

If any answer is no, rewrite.

---

## Before & after: a real case study

**The setup.** In April 2026, a two-person B2B sales team had two events on the calendar — a sponsored healthcare conference and a co-hosted dinner with Brex. The original plans were detailed, well-formatted, and ~140 lines each. They covered logistics, outreach timelines, talking points, budget, and ROI targets.

**What the triad diagnosis found:**

- No **pipeline hypothesis** — just a target at the bottom ("4-6 SQLs in 60 days")
- No **knock-out analysis** — the highest-leverage check (is this audience actually buyers, or vendors and consultants?) was nowhere in the plan
- **Tasks were logistics** ("update QR code", "print 1-pagers"), not analyses with hypothesis + owner + output
- **Post-event workplan was 7 bullets** for the most pipeline-critical phase of the entire event
- **Due dates had no times** ("this week", "day of")
- **No named DRI** per action
- **No kill list** (what are we explicitly NOT doing, and why)
- **No funnel projection** (attendees → conversations → meetings booked → SQLs → SQOs)
- **No risk register** (what if Brex delivers <10 attendees? what if the audience is mostly vendors?)

**The rewrite.** Same scope, same team, same budget. But structured through the triad:

- **Pipeline hypothesis stated explicitly** ("If we sponsor this event, we'll generate 4-6 SQLs / 2-3 SQOs / $150-300K pipeline because...")
- **Knock-out analysis sequenced FIRST** — audience quality verification by Apr 16, with explicit downgrade plan if it fails
- **SCR one-day answer** — 3 sentences capturing where the event sits in the broader pipeline picture
- **Explicit funnel with conversion rates** at every stage
- **6-column workplans** for pre-event, at-event, AND post-event (with post-event being the longest section — that's where pipeline is actually made)
- **Named DRI + date + time** on every line
- **Kill list** (no consultants in room, no pitch decks at booth, no follow-up to non-buyers)
- **Risk register** with mitigations

Same team. Same budget. Same two hours of planning. But now: a hypothesis-driven bet with named owners, a knock-out check that prevents wasted work, and a post-event workplan that makes pipeline instead of letting it evaporate.

The difference isn't the inputs. It's the operating system.

---

## Anti-patterns the triad eliminates

- ❌ Logistics checklists disguised as plans
- ❌ Goals without hypotheses ("fill 15 seats")
- ❌ Tasks without a single named DRI ("the team will handle")
- ❌ Due dates without times ("next week", "by Friday")
- ❌ Outputs that aren't dummied — if you can't sketch the chart, don't run the analysis
- ❌ Equal weighting — without a knock-out, the critical path is undefined
- ❌ Missing post-execution workplan — follow-up is where outcomes are made or lost
- ❌ "Boil the ocean" research before defining the problem
- ❌ Advocacy framed as analysis (fear/anger driving a priority)
- ❌ Meetings without agendas, decisions without RAPID clarity
- ❌ Issue without proposed solution ("just raising it")
- ❌ Generic narrative instead of pyramid-structured argument

---

## How to install this in your organization

This repo is structured to drop straight into any Claude Code workspace in ~5 minutes.

```
mckinsey/
├── README.md                           ← this file (the manifesto)
├── CLAUDE.md                           ← drop-in snippet for your project's CLAUDE.md
├── INSTALL.md                          ← step-by-step install guide (3 levels)
├── LICENSE                             ← MIT
├── skills/
│   ├── problem-solving/SKILL.md        ← the /problem-solving skill
│   ├── work-plan/SKILL.md              ← the /work-plan skill
│   └── mochary-method/SKILL.md         ← the /mochary-method skill
├── memory/
│   └── feedback_how_we_work_triad.md   ← optional persistent memory seed
└── examples/
    └── case-study-event-plan.md        ← before/after case study
```

**The 2-minute install:**

```bash
# 1. Clone this repo (or download the files)
git clone https://github.com/chefjefff/mckinsey.git

# 2. Copy the skills into your Claude Code skills directory
cp -r mckinsey/skills/* ~/.claude/skills/
# (or for a project-local install: mkdir -p .claude/skills && cp -r mckinsey/skills/* .claude/skills/)

# 3. Paste the contents of mckinsey/CLAUDE.md into your project's CLAUDE.md (at the top)
```

That's it. Your AI agents now default to the triad.

**For the full install (5 min, including persistent memory across conversations):** see [`INSTALL.md`](./INSTALL.md).

**Works with:** Claude Code, Cursor, or any AI IDE that reads markdown skill files + a CLAUDE.md equivalent.

---

## A note on sourcing and attribution

**This is not original thinking.** This is a packaging of three existing bodies of work into a portable operating system for AI-assisted work.

- `/problem-solving` is 100% distilled from **Charles Conn and Robert McLean's *Bulletproof Problem Solving***. If you find value here, buy their book. The 30 worked examples are exceptional and couldn't fit in a skill file.
- `/work-plan` is Step 4 of their framework, extracted because it's the most reached-for piece in day-to-day work.
- `/mochary-method` is distilled from **Matt Mochary's *The Great CEO Within*** and his [open-source Mochary Method Curriculum](https://mocharymethod.com/).

**What's original:** the recognition that these three disciplines form a complete operating triad, the packaging into portable skill files, the integration into Claude Code, and the insight that AI agents need these disciplines *more* than human-only teams (because they can produce plausible-but-hollow outputs at scale).

**License:** Free to use, modify, share, or deploy commercially. No attribution required to me. But please credit Conn, McLean, and Mochary if you publish derivatives — this is their work standing on their shoulders.

---

## Why this matters for AI-assisted work specifically

Human teams that skip these disciplines fail slowly — they burn a quarter on bad work, eventually someone notices, they course-correct.

AI-assisted teams that skip these disciplines fail **faster and more silently**. The agents produce 20 plans a day. The plans look professional. Nobody notices the missing hypotheses, the absent DRIs, the vague due dates — until the quarter ends and nothing moved.

**The AI doesn't know it's producing hollow work.** It's your job to install the operating system that forces rigor at the three layers where work breaks. Then your agents will write plans that survive Monday morning.

---

## Who this is for

- Founders and operators running on Claude Code, Cursor, or any agentic setup
- Ex-consultants who recognize these frameworks and want them codified for AI
- Product, growth, sales, and ops teams that use AI to scope work
- AI builders who are tired of their agents outputting beautiful logistics

---

## How to share this

**On LinkedIn:** share this `README.md` directly (or link to it). The manifesto is self-contained and reads in 5-10 minutes.

**In your org:** point at this repo. Anyone can clone it and drop the triad into their workspace in 5 minutes.

**As a talk or workshop:** the triad + 3-question test + case study form a 30-minute presentation. No permission needed.

---

## Credits

**Framework sources:**

- Charles Conn & Robert McLean — *Bulletproof Problem Solving: The One Skill That Changes Everything* (Wiley, 2019)
- Matt Mochary — *The Great CEO Within* + open-source Mochary Method Curriculum

**Integrator:**

- Jeffrey Zheng — ex-McKinsey consultant (Sydney), now running B2B enterprise sales at Superpower. Built this to make his two-person sales team + his AI agents operate like a McKinsey study team.

**Inspiration:**

- Dominic Barton, Barbara Minto, Barry Nalebuff, Dan Lovallo (problem-solving traditions)
- Sam Altman, Brian Armstrong, Naval Ravikant (Mochary-trained CEOs)
- The Claude Code team at Anthropic for building an agent system that deserves a proper operating system

---

*If this resonates: share the file, install the triad, and pressure-test your next plan against the 3-question test. If you find the triad useful, the real credit goes to Conn, McLean, and Mochary. I just wired them together.*

— **Jeffrey Zheng**
