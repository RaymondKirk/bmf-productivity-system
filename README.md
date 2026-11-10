# BMF Productivity System

**Notion workspace case study | Real system, synthetic demo records | Public case study **

I designed and use Build My Focus (BMF) as a personal operating system in Notion. Its Control Tower connects goals, actions, notes, daily planning, and weekly review. This repository documents the architecture and shows a public-safe example. The demo records are invented; they are not an export of my private workspace or a downloadable Notion template.

## The problem

Plans, tasks, and useful information can end up in separate places. A list of tasks alone does not show why the work matters, and notes can be hard to turn into action. I wanted one place to capture an idea, connect it to a goal, choose the next action, and review progress.

## My role and the solution

I designed the workspace structure, connected its databases, and organized the views around a recurring workflow:

1. **Capture:** Add an action or note quickly from the Control Tower.
2. **Clarify:** Give an action a status, priority, due date, and related goal where relevant.
3. **Focus:** Use the daily dashboard and action views to choose current work.
4. **Review:** Use weekly tracking to revisit goals, unfinished actions, and lessons.

The [data model](data-model.md) describes the public version of this system. The [sample records](sample-records.md) walk through one fictional project.

## What exists in the private workspace

| Component | Verified purpose | Public treatment |
| --- | --- | --- |
| Control Tower | Central navigation, quick capture, routine views, and links to the core databases | Described here; no private dashboard screenshot |
| BMF Actions | Tracks status, priority, due date, goal relation, blockers, parent tasks, and completion | Simplified synthetic records |
| BMF Goals | Connects goals and actions, with timeframes and current/completed views | Simplified synthetic records |
| BMF Notes | Captures source, type, topic, tags, and privacy choice | Simplified synthetic records |
| Daily Dashboards and Weekly Tracking | Supports planning and review | Workflow description only; no usage or outcome metrics claimed |


## Design choices

- **Goals and actions are linked.** A task can be traced to the result it supports.
- **Notes are distinct from actions.** A captured idea becomes an action only when there is a concrete next step.
- **Blockers are visible.** Actions can identify what they depend on rather than sitting silently overdue.
- **Daily and weekly views serve different decisions.** Daily planning asks what to do next; weekly review asks whether the work still serves the goal.
- **Privacy is part of the model.** The real Notes database includes a privacy field, and the public example contains no personal or client records.

## Portfolio walkthrough

The fictional example in [sample records](sample-records.md) shows a goal, two actions, one blocker, and a note. It demonstrates the relationship between records without implying that these exact entries exist in my private system.

## What I would show a Notion consulting client

1. A discovery map: what the client captures, decides, does, and reviews.
2. A small set of databases with clear ownership and naming.
3. A dashboard and views for the actual daily and weekly decisions.
4. A test in which a new user captures an item and finds the next action without guidance.
5. A handoff guide covering maintenance, privacy, and what to change as the workflow evolves.
