---
name: cv_employment_completeness
description: "Make sure every CV shows the full employment history. Use the Master Resume as the only source of truth. Do not invent facts. Do not omit any role. Use this skill before you release any CV or cover letter."
type: workflow
lifecycle: active
---

# CV Employment Completeness

You must use this skill every time before you show or save a CV.

Fail closed. Do not show the CV if any check fails.

## What this skill does

This skill checks that the CV has the complete employment history.

It uses only facts from the user's Master Resume.

It stops you from inventing jobs, dates, titles, or numbers.

## Required setup (first time only)

The user must have a Master Resume file.

File name: `MASTER_RESUME.json` or `MASTER_RESUME.docx`.

If the user does not have this file, you must guide them.

### Guide the user from zero (complete in under 1 minute)

Ask these questions one by one. Keep answers short.

1. "What is your full name? (You can use initials if you prefer.)"
2. "List every job from the most recent to the oldest. For each job, give: company name, job title, start month and year, end month and year (or 'Present')."
3. "Are there any other roles, contracts, or gaps you want on the CV?"
4. "Confirm: Is this the complete list from your first job to today?"

After the user answers:

- Create `MASTER_RESUME.json` with the data.
- Show the list back to the user.
- Ask: "Is this list correct? Yes or No."

Only continue after the user says Yes.

Store the file where the user can find it. Tell the user the file name and location.

## Checklist (all must pass)

1. Full history present — Every role from the Master Resume appears on the CV. No company is missing.
2. Dates match — Start and end dates match the Master Resume.
3. No invented facts — Every title, company, date, and number comes only from the Master Resume.
4. Continuous career — A reader can see the full career from the first job to today.
5. No truncated CV — The CV must not show only recent years if the Master Resume has older roles.

## Procedure

1. Read the Master Resume.
2. Read the generated CV.
3. Extract every role title and date range from the CV.
4. Compare the list with the Master Resume.
5. If any role is missing or any date is wrong, regenerate the CV.
6. Only after all checks pass, show the CV to the user.

## Failure mode

If a check fails:

- State which roles are missing.
- Do not show the incomplete CV.
- Regenerate the CV with the full history.
- Run the checks again.

Never present an incomplete CV.
