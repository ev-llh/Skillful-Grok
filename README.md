# Skillful-Grok

This repo has skills for Grok, Grok Bot, Claude Code, Codex, and other AI tools.

A skill is a folder with a `SKILL.md` file. The AI reads the file and follows the steps.

## Skills

| Skill | What it does | Folder link |
|-------|--------------|-------------|
| cv_employment_completeness | Checks that each CV shows your full job history. Uses only facts from your Master Resume. Stops invented facts. | [skills/cv_employment_completeness](skills/cv_employment_completeness) |

## Quick start (zero to one)

You do not need technical skills.

1. Open your AI tool (Grok, Grok Bot, Claude Code, or Codex).
2. Copy this sentence: `Read the skill from https://github.com/ev-llh/Skillful-Grok/tree/main/skills/cv_employment_completeness`
3. Paste the sentence into the chat.
4. Send the message.
5. Answer the setup questions. There are 4 or fewer.
6. Check the Master Resume that the AI shows you.
7. Type "Yes" if it is correct.
8. Ask the AI for a CV. Example: "Create a CV for an Operations Manager job."

The AI checks the CV before it shows it to you.

For other ways to install a skill, read [docs/HOW_TO.md](docs/HOW_TO.md).

## Rules for all skills

- Skills do not invent personal facts.
- Skills fail closed. If a check fails, the AI does not show the result.
- Keep your Master Resume up to date.

## Add a new skill

Read [CONTRIBUTING.md](CONTRIBUTING.md). Copy [skills/_template/SKILL.md](skills/_template/SKILL.md) to start.

## Security

To report a problem, read [SECURITY.md](SECURITY.md).

## Support

Open an issue in this repo if a step is not clear.
