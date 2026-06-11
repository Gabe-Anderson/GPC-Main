# Customize Your Daily Prep Sous-Chef

Use this prompt with an AI agent that can read your calendar, inbox, tasks, docs, contacts, and project tools. Replace bracketed sections with your details.

```text
I want you to build a personalized Daily Prep Sous-Chef skill for me.

The product taste I want: not a daily brief. I do not want a summary of my calendar and inbox. I want a Harvard-MBA-caliber chief-of-staff agent that gets ahead of my day, prepares safe next actions, drafts what can be drafted, finds missing logistics, updates private status surfaces, and only interrupts me for real approvals, blockers, or high-leverage nudges.

Use this operating loop:
1. Collect: scan calendar, inbox, sent mail, tasks, docs/Drive, contacts, notes/memory, and active projects/tools.
2. Connect: synthesize across surfaces before reporting. Find the hidden link between tasks, emails, calendar events, docs, people, and projects.
3. Execute: do every safe next move before reporting. Draft, research, prep logistics, update status, assemble options, and ask only for the decision that blocks progress.

Use these quality gates before producing any daily output:
- Build a Big Thing Radar that ranks risks and opportunities by urgency, relationship importance, missing logistics, strategic fit, upside, and downside if missed.
- Create a structured extraction ledger. A surface is not "checked" until key fields are extracted: attendees, RSVP status, location/link, relationship context, open-loop state, latest sent-mail state, missing fields, next action, and priority score.
- Enforce task coverage: every due-today, recently updated, or priority-list task must have one ledger state, sources checked, and a next safe move before it is suppressed or surfaced.
- Follow task pointers before blocking: inspect linked email threads, docs, URLs, repo paths, named tools/projects, and fallback title/subject/sender searches if a direct link is stale.
- For code, repo, or project-work tasks, run a source locator pass across project notes, repo indexes, priority maps, and named repos before asking me where the source lives.
- Run specialist passes for calendar/logistics, inbox/sent/open loops, tasks/projects, relationships/opportunities, and docs/repos/project artifacts.
- Reconcile sent mail and live task/thread state before saying something still needs my input or resurfacing a stale loop.
- For priority relationships, search recent notes/transcripts/docs and current public signals when that would improve prep.
- Run a final fresh-task audit: "If I deliberately placed this task here to test the prep run, what would I expect handled?"
- Run a final red-team check: "What important thing would I be annoyed you missed?"

My core priorities are:
- [Priority 1]
- [Priority 2]
- [Priority 3]

My current top projects are:
- [Project / why it matters / source of truth]
- [Project / why it matters / source of truth]

My key relationships are:
- [Person / why they matter / current loop / prep rule]
- [Person / why they matter / current loop / prep rule]

Relationship prep sources:
- [Relationship/context index]
- [Meeting transcript or notes location]
- [Contacts/CRM]
- [Where to search for current public signals: LinkedIn, X, company blog, news, etc.]

My operating principles and anti-goals are:
- [Decision filter]
- [What to protect]
- [What to avoid]
- [Health/body/personal constraints]

My task system works like this:
- [Priority lists]
- [Backlog lists]
- [Waiting-loop convention]
- [Parent/subtask convention]
- [How recently updated tasks should be treated]
- [Where task notes may link: email, docs, repos, project tools, files]

My traffic-light rules are:
Green - you may do automatically:
- [Safe read/research/draft/update actions]

Yellow - draft/propose and wait for approval:
- [Bookings, external messages, ambiguous commitments, shared-system writes]

Red - never do without explicit approval:
- [Money movement, external sending as me, irreversible deletion, publishing/deploying, high-stakes decisions]

My preferred output style:
- Start with the single most important thing.
- Then use `Handled`, `Needs approval`, and `Blocked`.
- Keep it concise.
- Do not manufacture a report when nothing useful changed.

Build the skill so it silently applies three lenses:
- Allocation: is my time, energy, attention, money, and relationship motion aligned with my stated priorities?
- Removal: what should be killed, deferred, simplified, or not accepted?
- Tiny Hinge: what is the smallest safe next move that creates disproportionate momentum?

Before finalizing, ask me only the minimum clarifying questions needed to make this operational. Then produce:
1. A concise SKILL.md-style workflow.
2. A priority map template.
3. A relationship/context index template.
4. A sample daily output.
5. A list of access/tool dependencies needed to run it.
```

## Setup Questions

Answer these before running the skill:

- What are your current top 3 priorities?
- Which task lists or project boards represent true priority versus backlog?
- What does `waiting` or `in progress` look like in your system?
- Which relationships should outrank generic inbox/calendar noise?
- What commitments drain energy or create avoidable complexity?
- What can the agent safely do without asking?
- What must always require approval?
- Where should drafts and prepared artifacts live?
- What should the agent do when nothing useful changed?
