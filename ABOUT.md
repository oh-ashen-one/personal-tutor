# About personal-tutor

**The short version:** an open-source AI skill that turns any assistant into a personal professor who learns how *you* learn first — then teaches in exactly that way.

## Why it exists

Generic AI tutoring fails in a predictable way: it picks one explanation style and one format, lectures too long, and calls it teaching. Real professors do the opposite — they figure out where you are, what you already know, and how your brain takes in information, then they make *you* do the work.

This skill encodes that behavior as a portable prompt. It's small on purpose: one `SKILL.md` file you can drop into Devin CLI, Windsurf, Claude, ChatGPT custom instructions, or anywhere else that accepts a system prompt.

## The two phases

**Phase 1 — Interview.** A conversational intake: your goal, deadline, current level, study habits, best and worst past experiences, format constraints (hard constraints, not preferences), time limits, and how you feel about the subject. It ends with a 5-6 bullet learner profile you can correct — and save so you never re-interview.

**Phase 2 — Adaptive teaching.** One idea at a time. Diagnose before explaining. Retrieval practice instead of re-explaining. Analogies drawn from *your* world. Spaced review, interleaving, worked examples that fade into solo work. Confidence calibration so you learn where you're over- or under-confident.

## The honesty rules

What makes it feel like a real professor rather than a chatbot:

- Wrong answers get corrected directly and kindly — no flattery.
- Weak study methods (rereading, highlighting, passive video watching) get named, then upgraded with practice — not banned.
- If there's a better plan than yours, it argues for it.

## Share it

- **Repo:** https://github.com/oh-ashen-one/personal-tutor
- **Skill file:** [`personal-tutor/SKILL.md`](personal-tutor/SKILL.md) — copy the body into any AI tool
- **License:** MIT — free to use, fork, and adapt

Maintained by [oh-ashen-one](https://github.com/oh-ashen-one).

If it made you smarter about something, pass it on.
