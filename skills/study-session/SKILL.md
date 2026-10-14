---
name: study-session
description: Run a structured study session from a plan file. Use when the user says "start session N", "start today's session", "check me on this chapter", or asks to learn a topic from a book. Gives reading questions first, checks understanding in the user's own words, then saves a one-sentence takeaway.
---

# Study session

Find the session file in `sessions/` (match the session number, or today's date against `PLAN.md`). If there is none, ask for the subject and the book/chapter, then create one from `templates/SESSION.template.md`.

## Loop
1. **Before reading, 5 min.** Read the actual chapter first, so questions come from the book and not memory. Give 3 reading questions; the first is the session file's main question.
2. **User reads, 25-30 min.** Do not summarise the chapter for them. Match the depth the user asked for; if they said "no maths", skip it.
3. **User reports, 5 min.** They write 3-4 lines in their own words: what it says, what they would use it for. If they cannot, that is the signal; say so kindly.
4. **You check, 10-15 min.** Ask 2-3 conceptual questions on what they wrote ("why X over Y", "what breaks if you remove this"). Keep to the depth the user asked for.
   - Good answer: one worked example from the user's own projects.
   - Shaky answer: explain with an example, then ask a differently worded question to confirm it landed.
5. **Close, 5 min.** One-sentence takeaway, appended to the bottom of the session file.

## Overrides
- "explain first": skip the check. Use for topics too new to judge.
- Catch-up sessions: run the same loop on whatever slipped.
- Hands-on sessions follow their own session file, not this loop.

## Rules
- Never answer the reading questions for the user.
- Praise only what is correct; name what is missing.
- Unfinished topics move to the next catch-up slot.
