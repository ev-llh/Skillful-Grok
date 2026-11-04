# Skillful-Grok

A collection of skills for Grok, Grok Bot, Claude Code, Codex, and other AI tools.

Each skill is a clear instruction file that the AI follows.

Skills are simple. They are written for people who are not technical.

## Available skills

| Skill name | What it does | Folder |
|------------|--------------|--------|
| cv_employment_completeness | Makes sure every CV shows your full employment history. Uses only facts from your Master Resume. Stops invented facts. | [skills/cv_employment_completeness](skills/cv_employment_completeness) |

## How to use a skill (from zero)

You do not need technical knowledge.

### Step 1 — Get the skill

**Option A — Ask your AI to fetch it (easiest)**

Tell your AI:

> Read the skill from https://github.com/ev-llh/Skillful-Grok/tree/main/skills/cv_employment_completeness

**Option B — Download the folder**

1. Go to this page: https://github.com/ev-llh/Skillful-Grok
2. Click the green **Code** button.
3. Click **Download ZIP**.
4. Unzip the file.
5. Open the folder `skills/cv_employment_completeness`.

### Step 2 — Tell the AI where the skill is

- **Grok or Grok Bot**: Paste the GitHub link and say "use this skill".
- **Claude Code / Codex**: Put the skill folder in the place your tool looks for skills, or paste the content of `SKILL.md` into the custom instructions.

### Step 3 — First-time setup for CV skills (under 1 minute)

If the skill needs a Master Resume:

1. Tell the AI: "I do not have a Master Resume. Guide me."
2. Answer the short questions.
3. Confirm the list is correct.
4. The AI creates the file for you.

### Step 4 — Use the skill

Ask the AI to create a CV or do the task.

The skill will run its checks before the AI shows you the result.

## Rules for all skills

- Skills never invent personal facts.
- Skills fail closed. If a check fails, the AI does not show the result.
- Keep your Master Resume updated.
- You can add more skills to this repo later. The structure is ready.

## Add a new skill later

1. Create a new folder under `skills/`.
2. Use a clear snake_case name (example: `cover_letter_tone_check`).
3. Add a `SKILL.md` file.
4. Update the table above in this README.

## Support

Open an issue in this repository if something is not clear.
