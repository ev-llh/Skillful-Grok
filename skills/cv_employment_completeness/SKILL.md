---
name: cv_employment_completeness
description: "Make sure every CV shows the full employment history. Use the Master Resume as the only source of truth. Do not invent facts. Do not omit any role. Use this skill before you release any CV or cover letter."
type: workflow
lifecycle: active
---

# CV Employment Completeness

Use this skill each time before you show or save a CV.

Fail closed. Do not show the CV if any check fails.

## What this skill does

This skill checks that the CV has the complete employment history.

It uses only facts from the user's Master Resume.

It stops you from inventing jobs, dates, titles, or numbers.

## First-time setup

Do this only if the user has no Master Resume.

The Master Resume file is `MASTER_RESUME.json`. A `MASTER_RESUME.docx` file also works.

Keep the setup to 1 minute or less. Ask at most 5 short questions. Ask one question at a time.

1. "What name goes on your CV? Initials are fine."
2. "List each job, newest first: job title, company, start month and year, end month and year or 'Present'."
3. "Do you want to add other roles, contracts, or gaps?"
4. "Is this the full list, from your first job to today?"

Then do these steps:

1. Create `MASTER_RESUME.json`. Use the format in `templates/MASTER_RESUME_TEMPLATE.json`.
2. Show the list to the user.
3. Ask: "Is this list correct? Yes or No."
4. If the user says No, fix the list and ask again.
5. Continue only after the user says Yes.
6. Save the file. Tell the user the file name and location.

Do not add facts that the user did not give. For a sample file, see `templates/example_MASTER_RESUME.json`. All data in it is fake.

## Checklist (all items pass)

1. Full history present — Every role from the Master Resume appears on the CV. No company is missing.
2. Dates match — Start and end dates match the Master Resume.
3. No invented facts — Every title, company, date, and number comes only from the Master Resume.
4. Continuous career — A reader can see the full career from the first job to today.
5. No truncated CV — The CV does not show only recent years if the Master Resume has older roles.

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
