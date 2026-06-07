# Obsidian + Claude: Minimum Viable System

The original guide lists 30 things. This is the 5 that deliver 80% of the value.

Each one covers a different layer. Skip any one and the system has a gap.

| Layer | What it solves |
|---|---|
| 1. Vault-Claude bridge | Claude can't help if it can't read your notes |
| 2. Three templates | Bad structure makes AI useless |
| 3. Capture workflow | Where value enters the system |
| 4. Morning Brief | Daily habit anchor |
| 5. Weekly Review | Where value compounds over time |

---

## 1. Vault-Claude Bridge

**The only non-negotiable.** Everything else depends on this.

Claude needs to read your vault without you copy-pasting files. There are two paths:

**Option A — MCP server (recommended if you use Claude Code)**
Install a local MCP server that points to your vault folder. Claude can then search and read notes as part of any workflow. This is the cleanest setup long-term.

**Option B — Folder access via Claude Projects**
In Claude.ai, create a Project and sync your vault folder as a knowledge source. Simpler to set up, slightly less flexible. Good starting point if you are not technical.

**What to do:**
- Pick one option and get it working before anything else
- Test it: ask Claude "what did I write about X?" and verify it finds the right note
- Do not move on until this works reliably

**Time:** 1–2 hours for Option A, 20 minutes for Option B.

---

## 2. Three Templates (Templater)

**The minimum structure Claude needs to be useful.**

You do not need 10 templates. You need exactly three, covering the three types of notes you will create most:

### Daily Note
```
# {{date}}

## Focus
- 

## Notes
- 

## Tasks
- [ ] 

## End of day
- 
```

### Meeting Note
```
# Meeting: {{title}} — {{date}}

**Attendees:** 
**Context:** 

## Notes


## Decisions


## Actions
- [ ] 
```

### Project Note
```
# {{project name}}

**Status:** Active | On hold | Done  
**Started:** {{date}}  
**Goal:** 

## Overview


## Open questions


## Next actions
- [ ] 
```

**Rules for every note:**
- One clear title
- At least one tag
- At least one link to another note once you have more than 20 notes

**Time:** 1 hour to install Templater and create the three templates.

---

## 3. Capture Workflow

**Where value enters the system.** Two triggers, one habit.

Most notes start as either a meeting or something you read. Both are currently time sinks — messy, unlinked, and forgotten a week later.

### Meeting cleanup
Immediately after a meeting, paste your rough notes and run this prompt:

```
Here are my rough notes from a meeting. 
Convert them into the meeting note format: Summary, Decisions, Actions (with owners and deadlines), 
and Related notes (suggest links based on topics mentioned).
Notes: [paste]
```

### Research intake
When you save an article, transcript, or idea, run this prompt:

```
Process this into a research note with: Key points (bullets), 
One-paragraph summary, Useful quotes, Related topics (for linking), 
Tags, and Follow-up questions.
Content: [paste]
```

**The habit:** Do not let raw notes sit in your inbox overnight. Process before you close the laptop.

**Time:** 10 minutes to set up the prompts. The workflow starts paying off on day one.

---

## 4. Morning Brief

**The daily habit anchor.** This is what makes the system feel alive instead of passive.

Every morning, Claude reads your recent notes and tells you where to start.

### Setup
Create a note called `_morning-brief-prompt.md` in your vault with this content:

```
Read my last 3 daily notes, any open tasks, and any active project notes.
Then create a short morning brief with:
1. What I was working on
2. What needs attention today (overdue or flagged)
3. One recommended focus for the morning

Be specific — reference actual note titles and task text.
Keep it under 200 words.
```

### How to use it
Each morning, open Claude with vault access and run the prompt. It takes 30 seconds. The output becomes your daily note header.

**Why this matters:** Without a daily trigger, the system is something you use occasionally. With it, the system is something you use every day — and a daily-use system improves, a sometimes-use system decays.

**Time:** 15 minutes to set up. 2 minutes per day to run.

---

## 5. Weekly Review

**Where the system compounds.** Without this, notes accumulate but never improve your thinking.

Do this every Friday, or Sunday evening. It takes 15–20 minutes.

### The prompt
```
Review my notes from this week (daily notes and any new notes created).
Give me:
1. What I completed or made progress on
2. What is still open or overdue
3. Any recurring problems or blockers worth naming
4. Two or three priorities for next week
5. Any ideas or notes worth connecting that I have not linked yet

Reference specific notes by title.
```

### What to save
The output of the weekly review becomes its own note: `Weekly Review — {{date}}`. Tag it `#review`. Over time, these become a searchable history of what you were focused on and what kept blocking you.

**Why this matters:** The Morning Brief tells you what to do today. The Weekly Review tells you if you are working on the right things at all. One without the other is incomplete.

**Time:** 15 minutes to set up the prompt and template. 20 minutes per week to run.

---

## Implementation Order

Do not start everything at once. Build in this sequence — each step makes the next one work better.

### Day 1 (2–3 hours)
1. Install Obsidian if you have not
2. Create folder structure: `Inbox / Projects / Areas / Archive`
3. Set up the vault-Claude bridge (pick Option A or B from step 1)
4. Install Templater, create the three templates
5. Create 5–10 real notes from current work using the templates

### Day 2 (1 hour)
6. Set up the two capture prompts (meeting cleanup, research intake)
7. Process one real meeting note and one real piece of research through them
8. Verify Claude can find and reference both notes

### Day 3 (30 minutes)
9. Create the `_morning-brief-prompt.md` note
10. Run your first Morning Brief
11. Use the output to structure your day

### End of Week 1
12. Run your first Weekly Review
13. Fix anything that felt awkward in the capture workflow or morning brief

### Week 2 and beyond
- Add a new workflow only when you feel friction that a workflow would solve
- Do not add plugins or complexity for their own sake

---

## What You Are Not Building (Yet)

These are worth knowing about but are not needed to get value from the system:

- Dataview and structured queries
- Kanban boards
- Graph analysis
- Zettelkasten conventions
- Vault cleanup automation
- Separate vaults

Add these later, if and when the core system is running smoothly and you feel a specific gap.

---

## The One Metric That Matters

After two weeks, ask yourself one question:

> Did a note I wrote earlier come back and actually help me this week?

If yes, the system is working. If no, the vault-Claude bridge is probably not functioning correctly — fix that before anything else.

---

## Why Only Five

The original guide describes the finished system.
This describes the system that makes you want to finish it.

Start here. The rest is optional.
