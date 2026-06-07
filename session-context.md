# Session Context — Obsidian + Claude Project

**Date:** 2026-06-07  
**Branch:** `claude/obsidian-claude-integration-pMm4O`  
**Repo:** `tesseractchain/basics`

---

## What We Did

1. **Captured raw ideas** from a 30-point guide on integrating Obsidian with Claude.
   Saved as: `obsidian-claude-integration.md`

2. **Critiqued the guide.** Key findings:
   - Core idea is solid: Obsidian = memory layer, Claude = reasoning layer
   - Main problem: describes a complete ideal system instead of a minimum viable one
   - Maintenance burden is underplayed
   - Privacy not mentioned (vault contents going to Claude API)
   - Plugin fragility not mentioned
   - Best ideas (Morning Brief, Research Intake, Feedback Loop) buried at same level as trivial ones
   - Chicken-and-egg problem: AI value assumes well-structured notes, but people need help *because* their notes aren't structured

3. **Distilled to 5 core components** that deliver 80% of the value.
   Saved as: `obsidian-claude-mvs.md`

---

## The 5 Core Components (Minimum Viable System)

| # | Component | Why it matters |
|---|---|---|
| 1 | Vault-Claude bridge (MCP or Claude Projects) | Nothing else works without this |
| 2 | Three templates via Templater (daily note, meeting, project) | Minimum structure for AI to be useful |
| 3 | Capture workflow (meeting cleanup + research intake prompts) | Where value enters the system |
| 4 | Morning Brief (daily prompt against recent notes) | Daily habit anchor |
| 5 | Weekly Review (Friday/Sunday prompt) | Where value compounds |

---

## Implementation Sequence

- **Day 1:** Bridge + templates + 5–10 seed notes
- **Day 2:** Capture workflow (process one real meeting + one piece of research)
- **Day 3:** First Morning Brief
- **End of Week 1:** First Weekly Review
- **Week 2+:** Add workflows only when you feel specific friction

## The One Success Metric

> Did a note I wrote earlier come back and actually help me this week?

If yes after two weeks, the system works. If no, fix the bridge first.

---

## Files in This Repo

| File | Contents |
|---|---|
| `obsidian-claude-integration.md` | Full 30-item guide, organized and cleaned up |
| `obsidian-claude-mvs.md` | Revised minimum viable system plan (start here) |
| `session-context.md` | This file |

---

## Where to Pick Up Next

Likely next steps (not started yet):
- Draft the actual template files for Obsidian
- Write the MCP server setup instructions in detail
- Create the specific prompt scripts for Morning Brief and Weekly Review
- Decide: personal use, publish as content, or build as a product?
