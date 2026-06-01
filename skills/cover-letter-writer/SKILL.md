---
name: cover-letter-writer
description: Writes a tailored, formal cover letter for a job application. Use this skill whenever the user provides a job description and wants a cover letter written, or says anything like "write me a cover letter", "cover letter for X", or "apply to Y". The skill reads the user's profile, selects the most relevant experiences and values for the role, and appends the letter to the user's cover letters Google Doc. Always invoke this skill for cover letter tasks — do not write cover letters inline without it.
---

# Cover Letter Writer

Orchestrates the cover letter writing process. The actual writing is handled by a dedicated subagent — your job here is to extract the key inputs and spawn it.

## What you need from the user

- The job description (full text, or the key parts)
- Company name and job title — extract from the JD if not stated explicitly

If the user hasn't provided the JD, ask for it before doing anything else.

## Spawn the writer subagent

Read the subagent instructions from:
`C:\Users\jigne\.claude\skills\cover-letter-writer\agents\writer.md`

Then spawn a subagent with:
1. The full subagent instructions from `writer.md` as context
2. The job description, company name, and job title filled in

The subagent handles everything from there: reading the profile, selecting relevant points, writing the letter, and appending to the Google Doc.

## After the subagent finishes

Relay its confirmation summary to the user — which points were selected, why, and the doc link.
