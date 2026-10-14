# study-plan

A Claude Code plugin that coaches you through book-based study sessions, for any subject. Claude gives reading questions first, makes you explain it back in your own words, checks your understanding, and saves a one-sentence takeaway.

## Install
    /plugin marketplace add saiprashanth802/study-plan
    /plugin install study-plan@study-plan

## Use
1. Copy `templates/PLAN.template.md` to `PLAN.md` and fill in your goal, slots and books.
2. `/start-session 1`: Claude reads the chapter, gives 3 reading questions, then waits while you read.
3. Write 3-4 lines in your own words; Claude asks 2-3 conceptual questions on them.
4. `/close-session`: saves a one-sentence takeaway to the session file.

Say "explain first" to skip the check on a topic that is too new to judge.

## Layout
    .claude-plugin/   plugin.json, marketplace.json
    skills/study-session/SKILL.md   the session loop
    commands/         /start-session, /close-session
    templates/        plan and session templates
    FORMAT.md         the loop, in plain words

Keep your books in `books/` (gitignored); they are never committed.

MIT licensed.
