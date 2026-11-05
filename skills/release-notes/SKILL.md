---
name: release-notes
description: Turns a list of completed user stories or tickets into release notes. Use when a Product Owner asks to "write release notes", "summarize what shipped this sprint" or "draft a release announcement". Not for writing user stories or sprint reports.
---

# Release Notes

Writes two versions of release notes from completed stories: one for end users and one short summary for stakeholders.

## Steps

1. Read the list of completed stories. Ignore any story marked not done.
2. Group stories into New, Improved and Fixed.
3. For users: write one plain sentence per item, describing the benefit, not the technical change. No ticket numbers.
4. For stakeholders: write 3 to 5 bullets covering the most important changes and any known issues.
5. If a story's benefit is unclear, list it under "Needs PO review" instead of guessing.

## Output format

```
## What's new
- ...
## Improvements
- ...
## Fixes
- ...

### Stakeholder summary
- ...

### Needs PO review
- ...
```

## Example

Input: "PB-101 Add CSV export to reports (done)", "PB-102 Fix login timeout on Safari (done)"
Output:
## What's new
- You can now export any report to CSV.
## Fixes
- Signing in on Safari no longer times out.

## Rules

- Never mention stories that are not done.
- Never invent features or benefits that are not in the stories.
