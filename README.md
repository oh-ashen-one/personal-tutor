# personal-tutor

An open-source [agent skill](https://github.com/oh-ashen-one/personal-tutor) that turns any AI assistant into your personal professor — one that learns how *you* learn before it teaches you anything.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## What it does

Most AI "tutors" dump information at you in one generic format. This skill does the opposite:

1. **It interviews you first.** Before teaching anything, it asks 2-3 questions at a time to build a learner profile: your goal and deadline, current level, study habits, what's worked and failed before, the formats you actually learn from (and the ones you *can't*), your time limits, and how you feel about the subject.
2. **It adapts to your profile.** Visual learner? You get diagrams and graphs. Hands-on? Problems first, theory second. Voice chat? Short spoken turns, quizzed out loud one question at a time. A format you said doesn't work is a hard constraint, not a preference.
3. **It makes you do the thinking.** Explain it back, predict what happens next, solve the problem. Hints first, answers last. If you can't explain it back, it re-teaches a different way.
4. **It uses techniques that actually work.** Retrieval practice, spaced review, interleaving, worked examples that fade into independent work, and confidence calibration checks.
5. **It's honest with you.** Wrong is corrected directly and kindly. Weak study methods (rereading, highlighting, passive video) get called out — and upgraded, not banned.

## Install

### Devin CLI / Windsurf / `.agents` standard

Copy or symlink the `personal-tutor/` directory into a skills folder:

```bash
git clone https://github.com/oh-ashen-one/personal-tutor.git

# Global (all projects)
mkdir -p ~/.config/devin/skills
cp -r personal-tutor/personal-tutor ~/.config/devin/skills/

# Or per-project (commit it to share with your team)
mkdir -p .devin/skills
cp -r personal-tutor/personal-tutor .devin/skills/
```

`~/.agents/skills/` and `.agents/skills/` work too — any tool that reads the `SKILL.md` standard picks it up.

### Any other AI (ChatGPT, Claude, etc.)

The skill is a self-contained prompt. Open [`personal-tutor/SKILL.md`](personal-tutor/SKILL.md), copy everything below the `---` frontmatter, and paste it into your system prompt, custom instructions, project instructions, or first message.

## Usage

Invoke it and start the interview:

```
/personal-tutor linear algebra for my exam in 3 weeks
```

Commands available any time:

| Command | What it does |
| --- | --- |
| `Quiz me` | Retrieval practice on what you've covered |
| `Teach it back` | You explain it, it grades you |
| `I'm stuck` | Switches explanations and slows down |
| `Exam mode` | Timed, realistic practice questions, no hints |
| `Update my profile` | Redo parts of the interview |

## Repo structure

```
personal-tutor/
├── README.md                  ← you are here
├── ABOUT.md                   ← shareable overview of the project
├── LICENSE                    ← MIT
└── personal-tutor/
    └── SKILL.md               ← the skill itself (the whole prompt)
```

## Contributing

Issues and PRs welcome — especially teaching tactics that worked on you. Keep the interview-then-teach structure and the honesty rules intact.

## License

[MIT](LICENSE) — use it, remix it, teach with it.
