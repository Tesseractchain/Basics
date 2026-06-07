# Obsidian + Claude Integration: Plugins, Workflows, and Setup

Most people use Obsidian as a notes app — writing things down, adding a few links, organizing folders.
Most people use Claude as a chatbot — ask a question, get an answer, start over the next day.

The real value starts when you connect the two.

- **Obsidian** becomes the memory layer.
- **Claude** becomes the reasoning layer.

Together, they turn your notes into a system you can actually work with.

---

## Part 1: The Core Plugins

### 1. Smart Connections
Best starting point for adding AI to a vault. Helps Claude find related notes instead of relying only on the current file — so old ideas, research, meeting notes, and project docs can surface when they're useful.

### 2. Copilot
AI chat experience inside Obsidian. Ask questions directly against your vault without jumping between apps. Notes and AI conversation in the same workspace.

### 3. Templater
Makes notes consistent. Use cases:
- Daily notes
- Meeting notes
- Project pages
- Content briefs
- Research summaries

Every important note starts with structure.

### 4. Dataview
Turns the vault into something closer to a database. Create live lists and tables from notes based on tags, dates, fields, projects, or status. Powerful when Claude can reason over structured notes instead of messy text.

### 5. Tasks
Manage to-dos inside notes with due dates, priorities, recurring tasks, and status. Work is not separated from thinking — projects, notes, and tasks stay connected.

### 6. Periodic Notes
Backbone of a time-based system. Daily, weekly, monthly, and quarterly notes give Claude a timeline of what happened, what changed, and what you were focused on.

### 7. Calendar
Makes daily notes easier to navigate. Simple but useful — when notes are connected to dates, Claude can help reconstruct work over time.

### 8. Kanban
Visual workflows for:
- Content pipelines
- Project stages
- Research queues
- Task planning
- Idea development

Claude can help update boards, summarize progress, and suggest next moves.

### 9. Obsidian Git
Version control for your vault. Keeps a history of notes — if something breaks, changes, or disappears, you have a way back.

### 10. Obsidian CLI
Command-line access changes everything for advanced setups. Once the vault can be searched, edited, and managed from the terminal, Claude Code or other agents can interact with it much more directly.

---

## Part 2: The Workflows That Make It Useful

### 11. Morning Brief
Claude checks recent daily notes, open tasks, and active projects, then creates a short start-of-day note with:
- What I was working on
- What needs attention today
- What is overdue
- What I should focus on first

Removes the "where do I start?" problem.

### 12. Meeting Cleanup
Drop rough meeting notes into Obsidian. Claude turns them into:
- Summary
- Decisions
- Action items
- Owners
- Deadlines
- Links to related projects

A messy note becomes a usable record.

### 13. Research Intake
When saving an article, video transcript, PDF, or idea, Claude processes it into a clean research note:
- Key points
- Useful quotes or claims
- Related notes
- Possible contradictions
- Tags
- Follow-up questions

Makes research reusable instead of disposable.

### 14. Weekly Review
Every Friday, Claude reviews the week and looks for:
- Completed work
- Missed tasks
- Active projects
- Recurring problems
- Ideas worth saving
- Priorities for next week

Instead of manually reviewing everything, you get a clean summary.

### 15. Idea Connector
When a new idea comes up, ask Claude to find related notes. The best insights usually come from connections you would not have searched for manually. This is where Obsidian becomes more than storage — it becomes a thinking system.

### 16. Project Kickoff
For every new project, Claude creates the starting structure:
- Project overview
- Goals
- Constraints
- Milestones
- Related notes
- Open questions
- Weekly update template

Starting clean makes the project easier to maintain.

### 17. Vault Cleanup
Once a month, Claude audits the vault and looks for:
- Notes with no links
- Inconsistent tags
- Old projects
- Missing metadata
- Unfinished drafts
- Duplicate ideas

Keeps the system from turning into a messy archive.

### 18. Book Notes System
After finishing a book, create one main note with highlights and thoughts. Claude connects it to:
- Projects
- Previous ideas
- Content topics
- Decisions
- Other books
- Useful frameworks

The book becomes part of the system instead of just another summary.

### 19. Argument Builder
When writing a post, proposal, or presentation, give Claude the main claim. It searches the vault for supporting material:
- Examples
- Past notes
- Research
- Data points
- Counterarguments
- Useful references

Makes writing much faster.

### 20. Decision Journal
Before important decisions, create a decision note:
- The situation
- Available options
- Assumptions
- Risks
- Expected outcome
- Final decision

Review later what happened. Over time, Claude can help identify patterns in how you make decisions.

---

## Part 3: The Advanced Setup

### 21. Claude Code + Vault Memory
Use the vault as long-term memory for Claude Code. Claude should know where the vault is, how notes are structured, and what conventions you use — so every task can start with relevant context.

### 22. MCP Server for the Vault
An MCP server lets Claude access the vault more cleanly. Instead of manually opening files or copy-pasting notes, Claude can search and read the vault as part of the workflow. This is the bridge between notes and automation.

### 23. Obsidian Skills
Reusable instructions for specific workflows:
- Process a meeting note
- Create a research summary
- Review a project
- Clean up a draft
- Build a content brief

Instead of prompting from scratch, trigger a known process.

### 24. AI-First Vault Rules
Every note should be easy for both humans and AI to understand:
- Clear titles
- Consistent tags
- Short summaries
- Useful links
- Simple metadata
- One idea per note when possible

Bad structure makes AI less useful.

### 25. Separate Vaults for Separate Contexts
Keep contexts from mixing. Separate vaults for:
- Personal life
- Work projects
- Learning
- Content
- Clients

Claude should only access the vault that matters for the task.

### 26. Nightly Processing Routine
At the end of the day, Claude reviews the inbox folder:
- Clean up rough notes
- Add tags
- Link related notes
- Move notes to the right folders
- Create a short daily summary

Wake up to a cleaner vault.

### 27. Graph Review
Obsidian's graph view is not just visual decoration. Claude can help identify:
- Central notes
- Isolated notes
- Clusters
- Weakly connected topics
- Places where new links should exist

This helps improve vault structure.

### 28. Zettelkasten + AI
Atomic notes work well with AI. When each note contains one clear idea, Claude can combine them in better ways — following chains of connected ideas instead of reasoning from one huge document.

### 29. Vault-Powered Claude Projects
Important parts of the vault become knowledge sources for Claude projects:
- Marketing notes → content project
- Finance notes → budgeting project
- Product notes → strategy project
- Research notes → writing project

Each Claude project gets the slice of knowledge it needs.

### 30. Feedback Loop
When Claude creates something useful, save it back into Obsidian:
- Summary
- Decision
- Draft
- Framework
- Checklist
- New idea

The vault gets smarter every time you use it.

---

## My Actual Stack

| Tool | Role |
|---|---|
| Obsidian | Notes and long-term memory |
| Smart Connections | AI-powered retrieval |
| Templater | Consistent note formats |
| Dataview | Structured views |
| Tasks | Action items |
| Periodic Notes | Daily and weekly rhythm |
| Claude | Reasoning and writing |
| Claude Code / MCP | Automation |

The system is not complicated. The hard part is setting up the first few workflows and actually using them every day.

---

## How to Start From Zero

Do not install everything at once. Build in this order.

### Hour 1
- Install Obsidian
- Create basic folder structure: `Inbox / Projects / Areas / Resources / Archive`
- Install Templater, create templates for daily notes and meeting notes

### Hour 2
- Install Smart Connections
- Add 5–10 real notes
- Ask Claude questions against your vault and see what it can find

### Hour 3
- Set up one MCP or local vault access method
- Goal: let Claude search and use notes without constant copy-paste

### Day 2
- Create 10–20 useful notes from current work
- Each note needs: clear title, useful tags, at least one link, enough context to make sense later

### Day 3
- Create your first workflow: the **Morning Brief**
- It should read recent notes, open tasks, and active projects, then create a short daily plan

### Week 1
- Add Dataview and Periodic Notes
- Start daily notes and one weekly review

### Week 2
- Improve the system
- Add cleanup, research intake, project kickoff, or content workflows based on what you actually do

---

## Why This Matters

> Obsidian without AI is powerful, but manual.
> Claude without Obsidian is useful, but forgetful.
> Together, they solve each other's biggest weakness.

- Obsidian gives Claude memory.
- Claude gives Obsidian intelligence.

You stop starting from zero.
You stop losing ideas in random notes.
You stop copy-pasting context every day.
You build a system where every note makes the next answer better.

Most people will keep using both tools separately. The advantage comes from connecting them.
