# Daily Prep Sous-Chef

An agentic alternative to daily briefs.

Most daily AI summaries are weak because they repeat your calendar, inbox, and task list back to you. A Daily Prep Sous-Chef should operate more like a Harvard-MBA-caliber chief of staff: sharp, forward-looking, commercially aware, personally aware, and biased toward removing friction before you feel it.

The job is not to summarize your day. The job is to prepare it.

## Core Idea

Run `Collect -> Connect -> Execute`.

- `Collect`: scan the surfaces that shape the day - calendar, inbox, sent mail, tasks, docs, contacts, notes, active projects, and tools.
- `Connect`: synthesize across surfaces before reporting. Find the link between a task, email, calendar hold, document, person, project, and priority.
- `Execute`: do every safe next move before interrupting the user. Draft, research, prep logistics, update status, assemble options, and ask only for the decision that blocks progress.

## What Makes This Different

A daily brief says:

> Here is what is on your calendar.

A daily prep sous-chef says:

> I found the unclear dinner logistics, drafted the confirmation text, checked the reservation path, updated the related task, and need one approval from you.

The taste is:

- Execution over briefing.
- Chief-of-staff posture, not passive assistant behavior.
- Harvard-MBA-caliber synthesis: commercially sharp, context-aware, priority-sensitive.
- Structured extraction before output: calendar, tasks, relationships, and projects become decision objects, not vibes.
- Big Thing Radar: rank risks and opportunities before writing the digest.
- Specialist passes for calendar/logistics, inbox/sent loops, tasks/projects, relationships/opportunities, and docs/repos.
- Tasks as inputs and status surfaces, not the product.
- Traffic-light autonomy: green automatic, yellow drafted/proposed, red explicit approval.
- One thing first, not a dashboard.
- Quiet when nothing useful changed.
- Priority-aware, not equal-weight.
- Next-72-hour logistics to prevent day-of scrambles.
- Sent-mail reconciliation so stale loops do not keep resurfacing.
- Priority relationship prep using relationship context, recent notes/transcripts when available, and current public signals when useful.
- Regression checks against past misses plus a final red-team question: "What important thing would the user be annoyed I missed?"
- Parent-task integrity for active projects.
- Personal operating-system awareness without creating a parallel ritual.
- Allocation / Removal / Tiny Hinge:
  - `Allocation`: is time, energy, attention, money, and relationship motion aligned with the user's stated priorities?
  - `Removal`: what should be killed, deferred, simplified, or not accepted?
  - `Tiny Hinge`: what is the smallest safe next move that creates disproportionate momentum?

## Files

- [`SKILL.md`](SKILL.md) - the generalizable skill.
- [`CUSTOMIZE.md`](CUSTOMIZE.md) - prompt and setup questions for personalizing it.
- [`examples/sample-output.md`](examples/sample-output.md) - example output shape.
- [`references/taste-extraction.md`](references/taste-extraction.md) - product taste notes and anti-patterns.

## How To Use

1. Read [`CUSTOMIZE.md`](CUSTOMIZE.md).
2. Fill in your priorities, traffic-light rules, task system, key relationships, and tool access.
3. Give the customization prompt to your AI agent.
4. Run the skill manually for 3-5 mornings before automating.
5. Judge it by artifacts prepared and decisions clarified, not by summary polish.

## Safety

The skill assumes clear action gates.

- Green: safe reading, synthesis, drafting, research, private status updates.
- Yellow: draft/propose and wait for approval.
- Red: never automate without explicit approval.

Do not let an agent send messages, book, buy, delete, publish, deploy, merge, move money, or make high-stakes decisions unless you have explicitly authorized that exact action.
