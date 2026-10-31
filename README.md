# Software Engineering Journey

My self-taught path from zero coding experience to remote full-stack software engineer, one week at a time.

This repo is my public learning log. Every week I study a new topic, build something with it, and push the notes and the project here. The plan runs for 52 weeks.

## The Roadmap

The full plan is in [`week_1_to_52_software_engineer_roadmap.pdf`](week_1_to_52_software_engineer_roadmap.pdf). It's split into stages:

| Stage | Weeks | Focus |
|-------|-------|-------|
| 1  | 1–6   | Computer science basics, the terminal, Git & GitHub |
| 2A | 7–12  | Semantic HTML5, modern CSS, responsive design |
| 2B | 13–18 | Core JavaScript, the DOM, async & APIs |
| 3A | 19–26 | React & TypeScript |
| 3B | 27–34 | Backend with Node.js, Express & PostgreSQL |
| 4A | 35–42 | Capstone portfolio & open source |
| 4B | 43–52 | Interview prep & remote job search |

**Weekly rhythm (15–20 hours):**
- **Mon–Fri, 2h/day:** study, code, then commit with a short log
- **Saturday, 3.5h:** build the week's project from scratch
- **Sunday, 1.5h:** review, refactor, write it up, deploy

## Progress

| Week | Topic | What I built | Status |
|------|-------|--------------|--------|
| [1](week_1/) | Computational thinking & setup (CS50x Week 0) | Pseudocode exercises, search notes, *The Dragon's Choice* Scratch game | ✅ Done |
| 2 | Variables, conditionals & loops (CS50x Week 1) | — | ⏳ Next |

## Week 1: Computational Thinking & Setup

**Plan:** [`week_1/week_1_day_by_day_study_plan.pdf`](week_1/week_1_day_by_day_study_plan.pdf)

### Notes — [`week1-notes.md`](week_1/week1-notes.md)
- Step-by-step pseudocode for three everyday tasks: finding a name in a phone book, joining friends for a game of Aion 2 on Discord, and picking the right audio and subtitles for an anime
- Linear search vs. binary search, with Python examples and why O(log n) beats O(n) as data grows

### Project — *The Dragon's Choice* (Scratch)

[`week_1/scratch hero game/`](week_1/scratch%20hero%20game/)

A choose-your-own-adventure story built for CS50x Problem Set 0. The King sends the hero to slay a dragon and rescue the princess, but nothing in the cave is what it seems. Every choice you make sends the story down a different path, and there are several endings to discover.

**What it uses:**
- 5 sprites (Hero, King, Princess, Dragon, Egg) and 6 backdrops
- Variables to track your choice, the current ending, and how many endings you've found
- Conditionals (`if` / `if-else`) to branch the story
- Loops (`repeat`, `repeat until`, `forever`)
- A custom block with an input that asks a question and checks the answer
- Broadcasts so the characters react to each scene

**How to play:**
1. Download [`The Dragons Choice.sb3`](week_1/scratch%20hero%20game/The%20Dragons%20Choice.sb3)
2. Open [scratch.mit.edu/projects/editor](https://scratch.mit.edu/projects/editor/) and choose **File → Load from your computer**
3. Click the green flag and make your choices

## Repo Structure

```
software-engineering-journey/
├── README.md
├── week_1_to_52_software_engineer_roadmap.pdf
└── week_1/
    ├── week_1_day_by_day_study_plan.pdf
    ├── week1-notes.md
    └── scratch hero game/
        ├── The Dragons Choice.sb3
        └── sprite and backdrop images
```

## Main Resources

- [Harvard CS50x](https://cs50.harvard.edu/x/)
- [The Odin Project](https://www.theodinproject.com/)
- [MDN Web Docs](https://developer.mozilla.org/)
- [GitHub Skills](https://skills.github.com/)
- [Exercism JavaScript Track](https://exercism.org/tracks/javascript)

---

*Week 1 of 52. Follow along as the repo grows.*
