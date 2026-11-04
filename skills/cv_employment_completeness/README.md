# How to use the CV Employment Completeness skill

## What you need

- A Master Resume file named `MASTER_RESUME.json` or `MASTER_RESUME.docx`.
- An AI tool that can read skill files (Grok, Grok Bot, Claude Code, Codex, or similar).

## First-time setup (under 1 minute)

1. Open your AI chat.
2. Tell the AI: "Use the cv_employment_completeness skill. I do not have a Master Resume yet. Guide me."
3. Answer the questions the AI asks.
4. Confirm the list is correct.
5. The AI creates the Master Resume file for you.

## Everyday use

1. Make sure the AI has access to the skill file and your Master Resume.
2. Ask the AI to create a CV for a job.
3. The AI will check the full employment history before it shows the CV.
4. If something is missing, the AI will fix it before you see the result.

## Where to put the skill file

### Grok / Grok Bot
Tell the bot: "Read the skill from https://github.com/ev-llh/Skillful-Grok/tree/main/skills/cv_employment_completeness"

### Claude Code or Codex
1. Download the folder `skills/cv_employment_completeness`.
2. Put the folder in the skills directory that your tool uses.
3. Or paste the content of `SKILL.md` into the custom instructions.

## Tips

- Keep your Master Resume updated when you change jobs.
- Never let the AI invent dates or job titles.
- The skill stops incomplete CVs from being shown.
