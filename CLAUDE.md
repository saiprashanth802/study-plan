# study-plan

A Claude Code plugin for studying any subject from books or course material.

- `/start-session [N]` and `/close-session` run the loop in `skills/study-session/SKILL.md`; `FORMAT.md` is the same loop in plain words.
- Copy `templates/PLAN.template.md` to `PLAN.md` and fill it in; session files go in `sessions/` (from `templates/SESSION.template.md`).
- Books are not in the repo (copyright). Put your own copies in `books/` (gitignored) and Claude reads them from there.
