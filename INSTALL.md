# Install Guide — Think / Plan / Operate

*5 minutes from zero to installed. No dependencies.*

---

## The 3-level install

Pick the level that matches how deep you want to go.

| Level | Time | What you get |
|-------|------|--------------|
| **1. Minimum viable** | 2 min | Agents default to the triad in this project |
| **2. Standard** | 5 min | Triad + persistent memory across conversations |
| **3. Full deployment** | 15 min | Triad wired into all your custom agents |

---

## Level 1: Minimum viable install (2 minutes)

### Step 1 — Get the files

```bash
git clone https://github.com/chefjefff/mckinsey-mochary.git
cd mckinsey-mochary
```

Or download as a ZIP from the GitHub repo page and extract.

### Step 2 — Install the three skills

Copy the three skill directories into your Claude Code skills folder.

**For a project-local install** (skills only apply to this one repo):

```bash
# From the root of the project you want to install into
mkdir -p .claude/skills
cp -r /path/to/mckinsey-mochary/skills/* .claude/skills/
```

**For a global install** (skills apply to every Claude Code session):

```bash
mkdir -p ~/.claude/skills
cp -r /path/to/mckinsey-mochary/skills/* ~/.claude/skills/
```

**For a Claude Code plugin** (distribute to a team):

Place each skill directory under `<your-plugin>/skills/`.

### Step 3 — Add the CLAUDE.md content

Open this repo's `CLAUDE.md`. Copy the entire file. Paste it at the top of your project's `CLAUDE.md` (or create a new `CLAUDE.md` if none exists).

That's it. Next time you open Claude Code in this project, the agents will default to the triad.

**Verify:** Type `/problem-solving` or `/work-plan` or `/mochary-method`. They should all be available.

---

## Level 2: Standard install (5 minutes)

Everything in Level 1, plus persistent memory so the triad loads into every future conversation.

### Step 3 — Install the memory seed

Claude Code maintains a per-project memory system. To make the triad load automatically in every conversation, drop in the memory seed:

```bash
# Find your project's memory directory. The path is:
# ~/.claude/projects/<slug-of-your-project-path>/memory/

# Example for a project at /Users/you/my-project:
MEMORY_DIR=~/.claude/projects/-Users-you-my-project/memory
mkdir -p "$MEMORY_DIR"

# Copy the memory file
cp /path/to/mckinsey-mochary/memory/feedback_how_we_work_triad.md "$MEMORY_DIR/"

# Update the MEMORY.md index
cat >> "$MEMORY_DIR/MEMORY.md" << 'EOF'

## 🧭 HOW WE DO WORK (foundational triad — always on)
- [feedback_how_we_work_triad.md](feedback_how_we_work_triad.md) -- /problem-solving + /work-plan + /mochary-method are the always-on operating foundation. Think + Plan + Operate. It is the work itself.
EOF
```

(If you're not sure what your project slug is, open Claude Code in the project once — it'll create the directory. Then find it with `ls ~/.claude/projects/`.)

### Step 4 — Verify

Restart your Claude Code session. The first thing Claude should know is "the triad is the operating default." Test by asking:

> "I want to plan a launch event. How do you approach it?"

The response should reference `/work-plan`, lead with a hypothesis, and ask about knock-out analyses — not dive into a logistics checklist.

---

## Level 3: Full deployment (15 minutes)

Everything in Level 2, plus wiring the triad into your existing custom agents so each agent reaches for all three skills by default.

### Step 5 — Update your agent files

For each custom agent that produces plans, projections, or strategic outputs (orchestrators, strategists, planners, reviewers), add a **"HOW YOU DO WORK"** section near the top.

Pattern to paste (customize the "Use when..." lines for the agent's domain):

```markdown
## 🧭 HOW YOU DO WORK (foundational triad — always on)

Three skills form your operating foundation for every output you produce.

### `/problem-solving` — How you THINK
- Define the problem crisply before starting any output
- Disaggregate into MECE logic trees
- Use multiple cleaving frames when diagnosing
- Synthesize with pyramid principle

### `/work-plan` — How you PLAN
Every output carries these 8 elements:
1. Hypothesis
2. Knock-out analysis (FIRST)
3. SCR one-day answer
4. Funnel / projection with conversion math
5. 6-column workplan (Issue / Hypothesis / Analysis / Owner / Output / Due with time)
6. Kill list
7. Risk register
8. Pre-launch checklist

### `/mochary-method` — How you OPERATE
- DRI for every action
- Issue / Proposed Solution (never bring an issue without a proposed action + owner + date)
- Clean Escalation (facts + options + tradeoffs, not advocacy)
- Fear/Anger check on priorities
- Top Goal protection for highest-leverage work

### The 3-question test (run before handing over any output)

1. Thinking: Is the analytical structure clear? (`/problem-solving`)
2. Planning: Every activity tied to outcome with named owner + date + time? (`/work-plan`)
3. Operating: Clear DRI? Issue paired with solution? Facts-not-advocacy framing? (`/mochary-method`)

If any answer is no, rewrite.

Full methods: `/problem-solving`, `/work-plan`, `/mochary-method`.
```

### Step 6 — Wire the invocation

In your agent, add an explicit call-out at the start of its workflow:

> "Before producing any output, invoke `/work-plan` (with `/problem-solving` for analytical structure and `/mochary-method` for operating discipline)."

This makes the triad a mandatory first step, not an optional reference.

---

## How to verify the install is working

Run any of these and check the output structure:

**Test 1 — Scoping:**
> "Help me plan next quarter's B2B event strategy."

**What "working" looks like:** output leads with a pipeline hypothesis, identifies a knock-out analysis, includes a 6-column plan with DRIs + times, includes a kill list. Does NOT lead with "First, let's look at venues..."

**Test 2 — Strategic diagnosis:**
> "Why is our CAC up 30% this quarter?"

**What "working" looks like:** output builds a recursive issue tree, applies 5 Whys, uses "what would you have to believe?" testing on each branch. Does NOT just list 10 possible causes.

**Test 3 — Team operations:**
> "I need to give tough feedback to a direct report who missed targets."

**What "working" looks like:** output uses Mochary feedback format ("I noticed X → I felt Y → I'd love Z"), separates behavior from identity, includes fear/anger regulation check. Does NOT jump straight into a script.

If any of these tests fails, go back to Step 1 and verify the skill files are in the right location.

---

## Troubleshooting

**"The skills aren't showing up."**
Check `ls ~/.claude/skills/` (global) or `ls .claude/skills/` (project). You should see three directories: `problem-solving`, `work-plan`, `mochary-method`. If not, the copy step didn't work.

**"The agents aren't using the skills."**
Check that `CLAUDE.md` has the "HOW WE DO WORK" section. Claude Code loads CLAUDE.md into every conversation — if the triad isn't named there, agents won't default to it.

**"The memory isn't persisting."**
Memory is per-project. If you moved the project or renamed it, the slug changed. Find the new slug with `ls ~/.claude/projects/` and re-copy the memory file.

**"I'm using Cursor / a different AI IDE."**
The skill files are just markdown. Paste them into your system prompt or `.cursor/rules/` or equivalent. The triad is portable — Claude Code is just where it's easiest to install.

---

## Uninstall

Delete the three skill directories. Remove the CLAUDE.md snippet. Delete the memory file. That's it. Nothing else is touched.

---

## What next?

- Read the before/after case studies in [`examples/`](./examples/) to see the triad applied to real work
- Share the [`README.md`](./README.md) manifesto with your team or on LinkedIn
- Pressure-test your next plan against the 3-question test
- If you build something useful with this, tell me — I want to learn what works

— Jeffrey
