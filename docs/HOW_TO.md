# How to use a skill

This guide is for people who are not technical.

A skill is a folder with a file named `SKILL.md`. The AI reads the file and follows the steps.

The examples use the skill `cv_employment_completeness`. Use the same steps for other skills. Change the folder name.

## Way A: Ask Grok or Grok Bot to fetch the skill

1. Open Grok or Grok Bot.
2. Copy this sentence: `Read the skill from https://github.com/ev-llh/Skillful-Grok/tree/main/skills/cv_employment_completeness`
3. Paste the sentence into the chat.
4. Send the message.
5. Wait for the AI to confirm that it read the skill.
6. Say: "Use this skill."

This way also works in other AI tools that can read web pages.

## Way B: Download the ZIP from GitHub

1. Open https://github.com/ev-llh/Skillful-Grok in your browser.
2. Click the green **Code** button.
3. Click **Download ZIP**.
4. Open the downloaded file to unzip it.
5. Find the folder `skills/cv_employment_completeness`.
6. Give that folder to your AI tool. Use Way C for Claude Code or Codex.
7. For other tools, copy the text of `SKILL.md` into the AI instructions.

## Way C: Put the folder in Claude Code or Codex

Keep the folder name the same as the skill name. The folder holds `SKILL.md`.

### Claude Code

Personal skills work in all your projects.

1. Do Way B to get the folder.
2. Create the folder `~/.claude/skills/` if it does not exist.
3. Copy the skill folder into it. The result is `~/.claude/skills/cv_employment_completeness/SKILL.md`.
4. Start Claude Code.
5. Type `/cv_employment_completeness`, or ask for a CV.

Project skills work in one project only.

1. Open your project folder.
2. Create the folder `.claude/skills/` if it does not exist.
3. Copy the skill folder into it. The result is `.claude/skills/cv_employment_completeness/SKILL.md`.

Source: Anthropic, "Extend Claude with skills": https://code.claude.com/docs/en/skills

### OpenAI Codex

Codex uses the folder `.agents/skills`, not `.codex/skills`.

User skills work in all your repos.

1. Do Way B to get the folder.
2. Create the folder `~/.agents/skills/` if it does not exist.
3. Copy the skill folder into it. The result is `~/.agents/skills/cv_employment_completeness/SKILL.md`.
4. Start Codex.
5. Type `$cv_employment_completeness`, or run `/skills`.

Repo skills work in one repo only.

1. Open your repo folder.
2. Create the folder `.agents/skills/` at the repo root if it does not exist.
3. Copy the skill folder into it. The result is `.agents/skills/cv_employment_completeness/SKILL.md`.
4. Restart Codex if the skill does not show.

Source: OpenAI, "Build skills" (Codex): https://developers.openai.com/codex/skills

## First-time Master Resume setup (1 minute)

1. Say: "I do not have a Master Resume. Guide me."
2. Answer the questions. There are 4 or fewer.
3. Check the list that the AI shows.
4. Type "Yes" if it is correct.
5. The AI saves `MASTER_RESUME.json`.

To see the file format, open [templates/example_MASTER_RESUME.json](../templates/example_MASTER_RESUME.json). All data in it is fake.

## Everyday use

1. Say: "Create a CV for [job title] at [company]. Use the cv_employment_completeness skill."
2. The AI checks the full job history.
3. The AI shows the CV only after all checks pass.

## Update your Master Resume

1. Say: "Update my Master Resume. I have a new job."
2. Answer the questions.
3. Type "Yes" to confirm.
