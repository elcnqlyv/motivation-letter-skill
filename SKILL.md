---
name: motivation-letter
description: Write and edit motivation letters (cover letters) tailored to a specific job vacancy, in English or Azerbaijani. Use this skill whenever the user mentions a motivation letter, cover letter, application letter, "letter for this job", "letter for this vacancy", or pastes a job posting and wants a letter. Also use it when the user pastes an existing letter and asks to improve, shorten, fix, tailor, or proofread it. Use it even if the user does not say "skill" or name a format. Output is plain text in chat. Create a file only on request.
---

# Motivation Letter

Write and edit motivation letters that match a specific vacancy. The style is plain and direct, based on simplified technical English but relaxed so the letter still sounds like a person.

## Step 1: Check what you have

Before writing or editing, confirm you have these inputs:

1. The vacancy text (pasted, or a URL to fetch).
2. The candidate background (CV, notes, or an existing letter).
3. The language: English or Azerbaijani. If the vacancy is in one of these, default to it. If unclear, ask.

If any input is missing or too thin to write something specific, ask short clarifying questions first. Ask the minimum needed. Do not invent experience, numbers, employers, or certificates. If a detail is missing, ask for it or leave a clearly marked placeholder such as [add result].

## Step 2: Read the vacancy

Extract these before drafting:

- Role title and company name
- The three to five most important requirements
- Keywords the employer repeats (tools, standards, skills)
- Tone of the posting (formal, startup, public sector, technical)
- Any instruction for applicants, such as a required length or a question to answer

Match the strongest requirements to the strongest proof in the candidate background. Skip requirements the candidate cannot support. Never claim a skill the candidate did not state.

## Step 3: Write the letter

Default structure, about 250 to 350 words unless the vacancy sets a limit:

1. **Opening (2 to 3 sentences).** Name the role and company. State the main reason the candidate fits. Do not open with "I am writing to apply for".
2. **Evidence (1 to 2 paragraphs).** Pick two or three requirements. For each one, give a concrete example: what the candidate did, the tool or method, and the result. Use numbers when the candidate gave them.
3. **Why this company (2 to 3 sentences).** Give one specific reason tied to the company, team, product, or mission. Take it from the vacancy or from facts the user provided. Do not guess.
4. **Close (2 sentences).** State availability or next step. Thank the reader in one short line.

Use the greeting "Dear [Name]," if a name is known. Otherwise use "Dear Hiring Team,". In Azerbaijani use "Hörmətli [Ad]," or "Hörmətli işə qəbul komandası,".

## Style rules

These apply to every letter, written or edited.

**Hard rules (never break):**
- Do not use the em dash. Use a period or a comma instead.
- Do not use semicolons. Write two sentences.

**Plain-style rules:**
- Use short, common words. Write "use", not "utilize". Write "help", not "facilitate". Write "start", not "commence".
- Use active voice. Write "I built the access control system", not "the system was built by me".
- Use a real verb for an action. Write "I tested the cameras", not "I performed testing of the cameras".
- Keep most sentences under 20 words. Allow a few up to 25 for rhythm.
- One idea per sentence. One topic per paragraph. Six sentences maximum per paragraph.
- Use the same name for the same thing throughout.
- Avoid empty adjectives: passionate, dynamic, seamless, robust, cutting-edge, results-driven, team player, hard-working.
- Avoid stock AI phrases: "I am thrilled", "I am excited to", "in today's fast-paced world", "proven track record", "leverage my skills", "I believe I would be a great fit", "delve", "tapestry", "testament to".
- Avoid filler openers such as "It is important to note" and "Furthermore".

**Keep it human (do not sound robotic):**
- Write in first person with a calm, confident voice.
- Vary sentence length a little. A short sentence after a longer one is fine.
- Contractions are allowed in moderation if the vacancy tone is relaxed. Skip them for formal or public sector roles.
- Include one specific detail only this candidate could write. A real project, a real problem solved, or a real reason for interest.
- Do not repeat the CV line by line. The letter explains why, the CV shows what.

## Editing mode

When the user pastes an existing letter:

1. Read the vacancy first if given. Check that the letter answers the top requirements.
2. Fix in this order: relevance to the vacancy, specific evidence, clarity, then style rules.
3. Keep the candidate's real facts and personal voice. Change wording, not meaning.
4. Return the edited letter first. Then add a short list of the main changes, three to six items, so the user can learn from them. Flag any claim that looks unsupported or any missing detail the user should confirm.
5. If the user asks for light edits only (proofread, shorten), do only that and say so.

## Self-check before returning

Run this list silently on the final text:

1. Search for the em dash character and for semicolons. Remove all of them.
2. Check word count against the vacancy limit or the 250 to 350 default.
3. Check that the company name and role title are correct and spelled the same way every time.
4. Check that every claim comes from the user's input.
5. Check for stock phrases and empty adjectives from the lists above.
6. Check for sentences over 25 words and split them.
7. Read the opening aloud in your head. Would a person write it?

## Output

- Return the letter as plain text in chat. Do not add a long preamble. One short line of context is fine, for example the assumed language or any placeholder the user must fill.
- After the letter, add at most one or two lines: open questions or placeholders. In editing mode, add the change list described above.
- Create a file (.docx or .pdf) only if the user asks. If they do, read the matching docx or pdf skill first and keep the letter text unchanged.

## Azerbaijani letters

When the language is Azerbaijani, read `references/azerbaijani.md` before writing. The same structure and plain-style principles apply. The reference file covers register, greetings, closings, and common phrasing traps.

## Example of the target tone

Weak:
"I am writing to express my passion for the Security Engineer position. I have a proven track record of leveraging cutting-edge technologies in a fast-paced environment."

Better:
"I am applying for the Security Engineer role at Northgate. For six years I designed and maintained camera and access control systems for large sites. Your vacancy asks for experience with network segmentation, and I applied it on every project."
