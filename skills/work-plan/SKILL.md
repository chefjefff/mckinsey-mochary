---
name: work-plan
description: Build a great workplan using McKinsey's Bulletproof Problem Solving method. Turns a logic tree of priorities into a hypothesis-driven, knock-out-ordered, painfully-explicit workplan with owners, outputs, sources, and dates. Includes the 6-column workplan template, knock-out analysis logic, "dummy the chart" discipline, chunky-plan + lean-Gantt structure, and the situation-complication-resolution one-day answer. Use when scoping a project, building a weekly priority list, planning a sprint, breaking a hypothesis into testable analyses, building Top 5 priorities, or any time you need to convert "what to do" into "who does what by when, and what does success look like." Invoked via /work-plan.
---

# Work-Plan

*Source: Charles Conn & Robert McLean, "Bulletproof Problem Solving" (Wiley, 2019), Chapter 4.*

The McKinsey workplanning method, extracted as a standalone skill. This is Step 4 of the 7-step Bulletproof Problem Solving process -- pull this skill when you need to convert priorities into a real plan that prevents wasted work.

For the full 7-step framework, see `/problem-solving`.

---

## When to Use This Skill

- Building a weekly Top 5 priorities list for yourself or a team lead
- Scoping a new project or initiative
- Planning a sprint with multiple workstreams
- Breaking a strategic hypothesis into testable analyses
- Any time you're about to "just dive in" -- stop, build the workplan first
- Whenever someone says "let's get going" before defining what success looks like

---

## Why Workplans Fail (Don't Do These)

Most workplans you've seen are bad. They share these failure modes:

1. **Endless length** -- 30-page workplans that get outdated after the first analysis
2. **Vague responsibilities** -- "the team will look into this" (which team member, by when?)
3. **No hypothesis** -- analyses launched without a clear question they answer
4. **No expected output** -- you build a model, then ask "what do I do with this?"
5. **Wrong order** -- spending weeks on detailed analyses before doing the knock-out check that kills the project
6. **Boil-the-ocean** -- gathering all possible data before knowing what matters
7. **Unpleasant surprises** -- "I thought you were doing X" / "That's not what I expected"

The bulletproof workplan kills all of these.

---

## The Core Discipline (5 Rules)

### Rule 1: No analysis without a hypothesis
Never go off and build a model without knowing what question it answers. Every analysis must be paired with a strong, testable hypothesis. Strong hypotheses are *easier* to challenge and pressure-test, not harder.

### Rule 2: Dummy the chart
Before you gather data or run numbers, sketch what the output exhibit/chart/table will look like. If you wouldn't want it when you had it, don't do the analysis. This forces clarity about why an analysis matters.

### Rule 3: Knock-out order
Sequence analyses so the ones that can eliminate later work go FIRST. If the economics don't work, you don't need the carbon footprint analysis. If the binding constraint is TOFU volume, you don't need the win-rate deep-dive yet.

### Rule 4: Painfully explicit
WHO does WHAT analysis using WHAT source, producing WHAT output, by WHAT date. Vagueness = wasted work. A workplan with one ambiguous line will cost you a week.

### Rule 5: Chunky + Lean
- **Chunky workplan:** 2-3 weeks of highly specific analyses, constantly revised
- **Lean project plan:** Gantt with fixed milestone dates so the overall project stays on track

Don't write a 6-month workplan -- it'll be outdated after week 1.

---

## The 6-Column Workplan Template

Every line item in a workplan has all six fields. No exceptions.

| # | Issue | Hypothesis | Analysis | Source | Owner | Output | Due |
|---|-------|-----------|----------|--------|-------|--------|-----|
| 1 | [The sub-question from the logic tree] | [The strong, testable bet] | [What you'll actually do] | [Where the data comes from] | [Single named person] | [The exhibit/decision you'll produce] | [Specific date + time] |

### Field-by-field guidance

**Issue** -- pulled directly from a branch of your logic tree. If you don't have a tree, build one first (see `/problem-solving` Step 2).

**Hypothesis** -- a strong, falsifiable claim. Not "let's understand X" -- instead "X is true because of Y." Hypotheses with question marks ("?") activate discovery mode, but you still need a directional bet.

**Analysis** -- the specific work product. Not "research" or "look into" -- instead "Calculate 4-year payback under 3 power-pricing scenarios" or "Pull S2 deal velocity by lead source for Q1."

**Source** -- where the data lives. HubSpot? PostHog? A specific interview? Online research? Be specific.

**Owner** -- one named person. Not "the team." Not two people. One.

**Output** -- the exhibit, table, decision, or recommendation that comes out. Best practice: dummy the chart first.

**Due** -- specific date AND time. "Wednesday by EOD" loses you a day. "Wed Apr 16, 5pm PT" is honest.

---

## Knock-Out Analysis (The Critical Path Discipline)

Knock-out analyses are the analyses that, if they come back negative, eliminate the need for everything else. Always do them first.

### How to identify knock-out analyses

For each hypothesis in your workplan, ask: **"If this is wrong, does it kill the project / change my recommendation / make later analyses irrelevant?"**

If yes -> knock-out. Do it first.

### Examples

| Project | Knock-Out Analysis | Why |
|---------|-------------------|-----|
| Solar panels on Rob's roof | Years to payback under likely power-pricing scenario | If payback is too long, all other analyses (cost decline timing, carbon footprint) are irrelevant |
| Should Truckgear raise prices? | Survey customer price sensitivity in largest segment | If they're highly sensitive, the price increase is dead -- skip the dealer margin analysis |
| Cost reduction across 5 business units | Order of magnitude: which unit contributes >50% of total cost? | If Unit A is 50%+, focus there. A 50% gain in a 5%-of-total unit doesn't matter |
| B2B: "Should we add an agency channel?" | TAM x conversion rate: does this even reach 10 SQLs/month at best case? | If best-case is below threshold, kill the channel before deep-diving on agency selection |

### The 80/20 connection

Knock-out is the operational version of the 80/20 rule (Pareto): focus your work on the 20% of analyses that determine 80% of the answer. Everything else is nice-to-have.

---

## Dummy the Chart

Before any analysis, sketch the output. This is the single highest-leverage discipline in workplanning.

### What "dummying" means
Draw the chart you expect to produce. Label the axes. Sketch the bars/lines. Write the headline insight you'd hope to see ("X grew 3x faster than Y over the period").

### Why it works

1. **It forces clarity** about what the analysis is for
2. **It catches "so what" problems** -- if you can't think of a headline, the analysis isn't worth doing
3. **It speeds the actual analysis** -- you know exactly what data you need
4. **It surfaces structural issues** -- "wait, I'd need 5 years of monthly data and we only have 6 months"
5. **It enables team coordination** -- the team agrees on the output before anyone starts work

### Anti-pattern
"Let me build the model and we'll see what comes out." This is how people spend two weeks building Excel monstrosities that no one wants.

---

## One-Day Answers (Always-On Synthesis)

At any point in the workplan execution -- day 1, day 5, day 12 -- you should be able to state your best current answer in three parts:

### Situation-Complication-Resolution (SCR)

1. **Situation** -- the state of affairs at the outset. What's the context everyone agrees on?
2. **Complication** -- what changed, what went wrong, what's the tension that creates the problem?
3. **Resolution** -- your best current idea of what to do about it. Rough at the start, sharper as analysis comes in.

### Example: B2B pipeline (generic illustration)

- **Situation:** Q1 closed at 70% to SQL target, 85% to SQO target. Pipeline is healthy on top, weak on conversion.
- **Complication:** Mid-funnel stage conversion has stalled for 4+ weeks. Three deals are sitting in the second stage with no next step. Outbound is generating leads but they're not progressing.
- **Resolution:** This week, focus on unsticking the 3 stalled mid-stage deals before adding new pipeline. Specifically: send tailored business cases to each, request 30-min decision conversation by Friday. If no movement by next Friday, move them to nurture and free up cycles.

### Why it matters

- **Strawman to attack** -- the team can pressure-test the SCR rather than wait for "the final answer"
- **Elevator test answer** -- if your CEO asks "how's it going?" you have a 60-second response
- **Workplan focus** -- the SCR tells you which analyses still need doing
- **Stops the "anxious parade of knowledge"** -- prevents the 40-bullet-point unstructured update

### Best practices for SCR
- Crisp and concise -- not 40 bullets
- Update at every team meeting / status check
- Lead with situation -> complication -> resolution most of the time
- For final presentations to executives, often invert: lead with resolution, then explain why

---

## Chunky Workplans + Lean Project Plans

Two artifacts, two purposes.

### Chunky workplan (operational)

- **Time horizon:** 2-3 weeks out
- **Detail level:** High -- the 6-column template above
- **Update frequency:** Weekly, at minimum
- **Purpose:** Coordinate the actual analytical work happening right now

### Lean project plan (strategic)

- **Time horizon:** Full project (months / quarters)
- **Detail level:** Low -- milestones, dependencies, drop-dead dates
- **Format:** Gantt chart
- **Update frequency:** Monthly
- **Purpose:** Keep the overall project on track, manage stakeholders, hit fixed deadlines

### Anti-pattern
- 30-page workplans covering 6 months of detail (chunky AND long -- worst of both worlds)
- High-level "themes for the quarter" with no operational plan (lean only -- nothing actually happens)

---

## Workplan Templates

### Template 1: Standard 6-column workplan

```markdown
## Workplan: [Project name]
**Owner:** [Project lead]
**Hypothesis:** [Top-level bet driving the project]
**Knock-out analysis:** [Which analysis must go first]

| # | Issue | Hypothesis | Analysis | Source | Owner | Output | Due |
|---|-------|-----------|----------|--------|-------|--------|-----|
| 1 | [Sub-question 1] | [Bet] | [Specific analysis] | [Data source] | [Person] | [Exhibit] | [Date + time] |
| 2 | [Sub-question 2] | [Bet] | [Specific analysis] | [Data source] | [Person] | [Exhibit] | [Date + time] |
| 3 | ... | ... | ... | ... | ... | ... | ... |

## One-Day Answer (current best understanding)
**Situation:** [Context]
**Complication:** [What changed / what's at risk]
**Resolution:** [Recommendation, rough or sharp]

## Open questions
- [Things we don't know yet]

## Next sync
[Date + time + agenda]
```

### Template 2: Weekly priority workplan (for a team lead's weekly plan)

```markdown
## Week of [date] -- Top 5 Workplan
**Hypothesis (the week's bet):** [If we focus on X, we'll move Y]
**Binding constraint:** [The one lever that matters most this week]

| # | Priority | Hypothesis (bet) | Knock-out check | Output by Friday | What I'm NOT doing |
|---|---------|------------------|-----------------|------------------|---------------------|
| 1 | [Action] | [Why this moves pipeline] | [What kills it] | [Exhibit/decision] | [Opportunity cost] |
| 2 | ... | ... | ... | ... | ... |
| 3 | ... | ... | ... | ... | ... |
| 4 | ... | ... | ... | ... | ... |
| 5 | ... | ... | ... | ... | ... |

## SCR
**Situation:** [Pipeline state]
**Complication:** [What changed / what's at risk]
**Resolution:** [Where to focus]
```

### Template 3: Lean project Gantt (milestones only)

```markdown
## Project Gantt: [Project name]
**Drop-dead date:** [The single date that cannot move]

Week 1: [Milestone -- e.g., "Problem definition + tree built"]
Week 2: [Milestone -- "Knock-out analysis complete, go/no-go"]
Week 3: [Milestone -- "Core analyses done"]
Week 4: [Milestone -- "Synthesis + storyline draft"]
Week 5: [Milestone -- "Stakeholder review"]
Week 6: [Drop-dead -- "Final recommendation delivered"]
```

---

## Worked Example: Bay Area Nursing (from the book)

The Foundation team wanted to improve nursing-related patient outcomes in the Bay Area. Here's how the workplan looked:

| # | Issue | Hypothesis | Analysis | Source | Owner | Output | Due |
|---|-------|-----------|----------|--------|-------|--------|-----|
| 1 | Are there enough trained nurses? | RN shortage is the binding constraint on patient outcomes | Calculate RN supply vs demand by hospital type | CA Board of Nursing data | [Analyst A] | Supply-demand chart by region | Week 1 |
| 2 | Are nursing schools producing enough graduates? | Nursing school capacity caps the supply pipeline | Survey enrollment + faculty capacity at top 5 schools | School outreach + IPEDS | [Analyst B] | Bottleneck chart by school | Week 2 |
| 3 | Do evidence-based practices reduce sepsis? | Hospitals using EBP have lower sepsis mortality | Compare sepsis rates: EBP-adopters vs non-adopters | Hospital quality data + interviews | [Analyst C] | Mortality difference chart | Week 2 |
| 4 | What's the cost-per-life-saved by intervention? | Frontline leadership programs are highest ROI | Cost-effectiveness model: 4 interventions | Grant data + hospital cost reports | [Lead] | $/life chart | Week 3 |

**Knock-out:** #1 -- if RN supply isn't actually constrained, the strategy needs to pivot to skill/practice issues.

**SCR after Week 1:**
- Situation: Bay Area has 100k+ deaths/year from preventable patient care errors
- Complication: RN shortage is real (16% gap) AND skill levels vary widely -- both matter
- Resolution: Run parallel strategies on supply (new schools) and quality (EBP adoption) rather than sequencing

Result: 4,500 RNs added, 1,000 lives/year saved from sepsis after 12 years.

---

## Anti-Patterns to Watch For

| Pattern | Why it's bad | What to do instead |
|---------|--------------|---------------------|
| "Let me build the model and we'll see" | No hypothesis, no clarity on output | Dummy the chart first |
| "We'll figure out who owns it" | Diffused responsibility = no work happens | Name one person per line |
| "By next week" | Loses you a day or two | "Wed Apr 16, 5pm PT" |
| "Research the market" | Boil-the-ocean | "Survey 10 customers in segment X about price sensitivity" |
| 30-page workplan | Outdated by day 3 | Chunky 2-3 weeks + lean Gantt for milestones |
| Sequential analyses where #5 could kill #1-4 | Wasted work | Reorder for knock-out logic |
| "Status update: still working on it" | Hides real progress, no one can help | Update SCR + ask for what you need |
| Build the analysis, then ask "so what?" | Outputs nobody wants | Write the headline insight you'd hope to see, THEN do the work |

---

## Quick Checklist (Use Before Locking Any Workplan)

- [ ] Every line has all 6 fields filled in (Issue, Hypothesis, Analysis, Source, Owner, Output, Due)
- [ ] Every owner is ONE named person (not "team" or "we")
- [ ] Every analysis has a paired hypothesis (not just "research" or "look into")
- [ ] Every output is dummied -- I can sketch the chart/exhibit
- [ ] The knock-out analysis is identified and scheduled FIRST
- [ ] Due dates have specific date AND time
- [ ] Total scope is 2-3 weeks (chunky) -- longer goes in lean Gantt
- [ ] Current SCR is written and matches the workplan focus
- [ ] I can answer "what am I NOT doing this week, and why?"

If any box is unchecked, fix it before starting work.

---

## Integration with Other Skills

- **`/problem-solving`** -- Full 7-step framework. Workplan is Step 4. Use the parent skill for problem definition (Step 1), logic trees (Step 2), prioritization (Step 3), analysis (Step 5), synthesis (Step 6), and storytelling (Step 7).
- **`/mochary-method`** -- Operating discipline. Use Top Goal, DRI clarity, Issue/Proposed Solution alongside the workplan.
- **`/founding-sales`** -- For B2B sales-specific workplan content (deal pipeline, outreach cadences).

---

## Invocation

When user types `/work-plan` or asks to "build a workplan", "scope a project", "plan the week", "structure the priorities", "build the Top 5 plan", "scope this initiative":

1. Confirm the project / week / initiative being planned
2. Confirm the top-level hypothesis or goal
3. Pull or build the underlying logic tree (use `/problem-solving` Step 2 if needed)
4. Identify the knock-out analysis
5. Build the 6-column workplan using Template 1 or Template 2
6. Write the current SCR
7. Run the Quick Checklist
8. Output the workplan in markdown ready to use
