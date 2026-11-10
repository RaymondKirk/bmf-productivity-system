# Public data model

This is a simplified, buildable model based on the structure of my private BMF workspace. It omits personal fields, specialized views, and automations. Field names in the live workspace may differ from this public version.

| Database | Core fields | Relation | Useful views |
| --- | --- | --- | --- |
| Goals | Goal, type, timeframe, complete | One goal to many actions | Current, completed |
| Actions | Action, status, priority, due date, completion date, blocked by | Related goal; self-relation for blockers | Today, upcoming, blocked, completed |
| Notes | Note, type, topic, source, private | Optional related goal or action in a client adaptation | Inbox, by topic, private |
| Daily Review | Date, focus, selected actions, reflection | Actions | Today, past days |
| Weekly Review | Week, goal check, wins, obstacles, next changes | Goals and actions | Current week, archive |

## Key rules

1. Every active action has a status and a clear verb. Add a goal relation when it supports a defined goal.
2. A blocked action names the blocking action or decision and an owner for follow-up.
3. Notes can be kept without becoming tasks. Convert a note to an action when it contains a specific next step.
4. Mark a goal complete after reviewing the outcome, not simply because its linked actions are closed.
5. Review views should expose current work and stale work; they should not require users to browse the entire database.
6. Keep private notes and sensitive attachments out of a public demo or broadly shared client dashboard.

## Example acceptance checks

These are proposed checks for a public demo, not measured results from the private system.

- Capture a note and an action from the dashboard, then find both in their databases.
- Link an action to a goal and confirm the goal shows the related action.
- Mark an action blocked and identify the dependency in the blocked view.
- Complete an action and confirm it leaves the current-work view while remaining in history.
- Ask a first-time user to explain what matters today and how it connects to a goal.
