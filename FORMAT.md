# Book session format (default for every reading session)

Applies to every session with a "Read:" line. Hands-on sessions follow their own session file.

1. **Before reading, 5 min.** Claude gives 3 reading questions, so you read for answers. The first is the session file's main question.
2. **You read, 25-30 min.** On your own, from your copy (print, or a file in `books/`). Match the depth you asked for; if you said "no maths", skip it.
3. **You report, 5 min.** Write 3-4 lines in your own words: what the chapter says, and what you would use it for. If you cannot, say so; that is the useful signal.
4. **Claude checks, 10-15 min.** 2-3 conceptual questions on what you wrote ("why choose X over Y", "what breaks if you remove this"). Keep to the depth you asked for.
   - Good answer: Claude gives one worked example from your own projects (your own code, hardware or coursework).
   - Shaky answer: Claude explains it with an example, then asks a differently worded question to confirm it landed.
5. **Close, 5 min.** One sentence of takeaway, saved at the bottom of that session's file in this folder.

## Overrides
- Say "explain first" to skip the check. Use it for new topics you cannot yet judge, such as a subject you are meeting for the first time.
- Claude reads the actual chapter from `books/` before asking questions, so the questions come from the book, not from memory.
- Catch-up sessions: run the same loop on whatever slipped.

## How to start
Open Claude Code in this folder and say "start session N" (or "start today's session"). Claude finds the session file for that number or date.
