# Contributing

This repo has simple skills for AI tools.

## Add a new skill

1. Pick a snake_case name. Example: `cover_letter_tone_check`.
2. Create the folder `skills/<name>/`.
3. Copy [skills/_template/SKILL.md](skills/_template/SKILL.md) into the folder.
4. Set `name` in the frontmatter to the folder name.
5. Write a short `description`. Say what the skill does and when to use it.
6. Fill in each section of the template.
7. Add a row to the skills table in [README.md](README.md).
8. Open a pull request.

## Style rules (ASD-STE100)

- Use short sentences.
- Use active voice.
- Write one instruction in each sentence.
- Use simple words.
- Write for people who are not technical.
- Add a "First-time setup" section if the skill needs user data.

## Privacy

- Do not put personal data in any file. This repo is public.
- Use fake example data only. Examples: "Alex Example", "Example Corp", alex@example.com.
- Do not add links to private documents.

## Security

To report a security problem, read [SECURITY.md](SECURITY.md).
