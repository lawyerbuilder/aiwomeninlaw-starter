# How to write a decision note

- type: guide
- date: 2026-10-05
- related: [[MEMORY]], [[redesign]], [[sources]]

Write one note per decision, in this folder. Name the file with the date and a few words, for example `2026-10-17-sort-by-due-date.md`. Then add one line for it to the Decisions section of [[MEMORY]]. Fictional data only.

To change a decision, write a new note and add "replaced by" with a link to the new note in the old note's status line. Keep the old note.

## Template

Copy everything inside the box into the new note.

```text
# Sort requests by due date

- type: decision
- date: 2026-10-17
- status: current
- related: [[redesign]], [[sessions/2026-10-17]]

## Decision
Requests in the tool are listed by due date, earliest first.

## Reason
The team reviews requests in due-date order (S2).

## Options considered
- By date received: rejected, because urgent requests sank to the bottom.

## Who decided
Jane Example, after Claude listed the options.
```
