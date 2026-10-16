# Motivation Letter Skill

A Claude skill that writes and edits motivation letters (cover letters) for a specific job vacancy. It works in English and Azerbaijani.

## What it does

- Writes a new letter from a job vacancy and your background.
- Edits an existing letter so it matches the vacancy.
- Asks short questions first if the vacancy, background, or language is missing.
- Returns the letter as plain text in chat. It creates a Word or PDF file only when you ask.

## Writing style

The skill uses a plain style based on simplified technical English, relaxed so the letter still sounds like a person.

- No em dashes and no semicolons.
- Short, common words and active voice.
- Most sentences under 20 words.
- No empty adjectives or stock AI phrases.
- No invented experience, numbers, or certificates. Missing details become placeholders such as [add result].

## Repository structure

```
motivation-letter/
├── SKILL.md
└── references/
    └── azerbaijani.md
```

- `SKILL.md` holds the workflow, structure, style rules, editing mode, and self-check.
- `references/azerbaijani.md` holds register, greetings, closings, and phrasing traps for Azerbaijani letters.

## Installation

1. Zip the `motivation-letter` folder.
2. Rename the file to `motivation-letter.skill`.
3. In Claude, open the skill settings and upload the file.

## Usage

Paste a job vacancy and your CV or notes, then ask for a letter. Examples:

- "Write a motivation letter for this vacancy."
- "Edit my cover letter so it fits this job posting."
- "Write this letter in Azerbaijani."
- "Shorten this letter to 250 words."

## License

Add a license of your choice here, for example MIT.
