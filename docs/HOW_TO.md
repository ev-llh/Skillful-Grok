# How to use skills (detailed guide)

This guide is for people who are not technical.

## What is a skill?

A skill is a text file named `SKILL.md`.

The AI reads the file and follows the instructions inside it.

## Get a skill

### Method 1 — Tell the AI the link (recommended)

Copy this sentence and paste it to your AI:

Read the skill from https://github.com/ev-llh/Skillful-Grok/tree/main/skills/cv_employment_completeness

The AI will download and use the skill.

### Method 2 — Download the files yourself

1. Open https://github.com/ev-llh/Skillful-Grok in your browser.
2. Click the green button that says **Code**.
3. Click **Download ZIP**.
4. Open the downloaded file.
5. Find the folder `skills/cv_employment_completeness`.
6. Give that folder to your AI tool, or copy the text from `SKILL.md` into the AI instructions.

## Where to put the skill

| Tool | What to do |
|------|------------|
| Grok or Grok Bot | Paste the GitHub link. Say "use this skill". |
| Claude Code | Put the skill folder in the skills directory, or add the SKILL.md text to the project instructions. |
| Codex | Put the skill folder where Codex looks for custom skills, or paste the SKILL.md content into the system prompt. |

## First-time Master Resume setup (1 minute)

1. Tell the AI: "I do not have a Master Resume. Guide me."
2. Answer these questions when the AI asks them:
   - Your name (or initials)
   - Each job: company, title, start date, end date
   - Confirm the list is complete
3. Say "Yes" when the AI shows the list.
4. The AI saves `MASTER_RESUME.json` for you.

## Everyday use

1. Make sure the AI can read the skill and your Master Resume.
2. Say: "Create a CV for [job title] at [company]. Use the cv_employment_completeness skill."
3. The AI checks the full history before it shows the CV.
4. If a role is missing, the AI fixes it first.

## Update your Master Resume later

Tell the AI: "Update my Master Resume. I have a new job."

Answer the short questions. Confirm. Done.
