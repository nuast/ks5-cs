---
marp: true
theme: ks5
paginate: true
header: "OCR A-Level Computer Science · H446"
footer: "Welcome to Year 12"
---

<!-- _class: title -->

# Welcome to A-Level Computer Science

## Year 11 → Year 12 Transition

*[Date] · [School Name]*

<!--
PRESENTER NOTES
Keep this slide up while students settle. Play some lo-fi or coding
ambient music if you like. Aim for a relaxed, exciting atmosphere —
this is the first impression of the course.
-->

---

<!-- _class: section -->

# 🎉 You made it.

## Now the real fun begins.

<!--
Pause here. Let that land. This is meant to feel like a milestone, not
a formality. Tell them this course is genuinely exciting and that you're
looking forward to teaching them.
-->

---

## What is A-Level Computer Science?

- **Not** just programming — though we'll write a lot of it
- A blend of **theory**, **mathematics** and **practical skills**
- You'll understand *how computers actually work*, from transistors to the internet
- You'll build a **real software project** in Year 13

> This is one of the most useful and sought-after A-Levels you can take.

<!--
Briefly mention the three components:
  01 Computer Systems (written exam)
  02 Algorithms & Programming (written exam)
  03 Programming Project (coursework, 20%)
-->

---

## GCSE vs A-Level — What Changes?

<div class="columns">

**GCSE**
- Guided tasks
- Shorter programs
- Closed-book exams
- Mostly single-file scripts

**A-Level**
- Independent thinking required
- Multi-file projects
- Open-ended coursework
- You design the solution

</div>

> The gap is real — but completely bridgeable with the right habits.

<!--
Be honest about the step up. Reassure them that everyone finds it hard
at first, and that the jump is about approach and mindset, not raw talent.
-->

---

## What Makes a Good Computer Scientist?

- **Curiosity** — asking *why* and *how*
- **Persistence** — debugging is 70% of programming
- **Reading** — docs, articles, other people's code
- **Building** — the best way to learn is to make things
- **Breaking things** — deliberately, to understand them

> You don't need to be a genius. You need to be interested.

<!--
Tell a short story here — a student project, a bug you spent hours fixing,
something you built that surprised you. Make it personal.
-->

---

<!-- _class: section -->

# 🐍 What We'll Do Today

---

## Today's Plan

1. **Explore a small Python project** organised as a library
2. **See multiple interfaces** for the same program:
   - Command-line (terminal)
   - Command-line arguments (`argparse`)
   - Graphical interface (Tkinter)
3. **Look at projects** built by previous work experience students
4. **Discover how software grows** using Git and releases

<!--
Adjust this list to match what you actually have prepared. The key message
is: look how much you can do with the Python you already know when you
organise it well.
-->

---

## A Program, Three Interfaces

```
my_tool/
├── __init__.py          ← makes it a package
├── core.py              ← the actual logic lives here
├── cli.py               ← text menu interface
├── args.py              ← argparse interface
└── gui.py               ← Tkinter GUI
```

> The **same** core logic, completely separated from *how* the user interacts with it.

<!--
Walk through the folder structure. Open each file briefly in VS Code.
Show that core.py has zero UI code. This is the key insight: separation
of concerns. They will use this pattern throughout the course.
-->

---

## Demo: Running the Same Code Three Ways

```bash
# 1. Interactive CLI menu
python -m my_tool.cli

# 2. Command-line arguments
python -m my_tool.args --name "Alice" --count 5

# 3. Graphical interface
python -m my_tool.gui
```

> The computer doesn't care which interface you use — the maths is the same.

<!--
Live demo here. Keep it short — 3 minutes max. Let students ask one or
two questions after.
-->

---

## What Previous Students Built

<!-- Replace these bullets with real examples from your school. -->

- 🎮 A text-based adventure game with save/load (JSON files)
- 📊 A CSV analyser that produced charts with Matplotlib
- 🌐 A web scraper that tracked football scores
- 🤖 A Telegram bot that answered quiz questions
- 🔐 A password manager (terminal, with encryption)

> All of these started with *exactly* the Python you know now.

<!--
If you have screenshots or short videos, show them here. Real student work
is far more motivating than abstract examples.
-->

---

<!-- _class: section -->

# 📈 How Software Projects Grow

---

## From Script to Project

```
v0.1  →  single file, runs top-to-bottom
v0.2  →  functions added, code reused
v0.3  →  split into modules
v1.0  →  Git repository, README, tests
v2.0  →  multiple contributors, CI pipeline
```

> Every professional codebase started as a messy single file.

<!--
Draw the progression on the board or show a GitHub commit history
of a real open-source project. numpy, requests or flask are good examples
— zoom in on the early commits.
-->

---

## Git: Your Time Machine

```bash
git init          # start tracking a folder
git add .         # stage changes
git commit -m "Add login page"   # save a snapshot
git log --oneline # see the history
```

- Every **commit** is a snapshot you can return to
- Every **branch** is a safe space to experiment
- Every **release** is a tagged version you can share

> You will use Git for *every* piece of work in this course.

<!--
If students haven't used Git before, don't worry — we'll teach it
properly in the first few weeks. Today is just a taste.
-->

---

## GitHub Releases in the Wild

<!-- Optional: show a real GitHub releases page, e.g. Python or VS Code -->

- Open-source projects ship **versioned releases** (v1.0, v2.3.1 …)
- Each release has a **changelog** — what changed and why
- You can download any previous version instantly
- This is how the whole software industry works

> By the end of Year 13, you'll have your own release history.

<!--
Open github.com/python/cpython or similar and scroll to Releases.
Show them v3.12, v3.11, etc. and click on one to see the release notes.
This makes the abstract concept of version control feel real.
-->

---

<!-- _class: section -->

# 🔭 What You'll Build Over Two Years

---

## Year 12 — Foundations

- **Python** — data structures, algorithms, OOP
- **Computer Systems** — processors, memory, operating systems, networks
- **Computational Thinking** — abstraction, decomposition, pattern recognition
- **Small projects** — practise, practise, practise

---

## Year 13 — Going Deeper

- **Advanced algorithms** — sorting, searching, graph traversal
- **Functional programming** — a completely different way of thinking
- **Databases, security, ethics**
- **Programming Project (NEA)** — your own full application, 20% of the grade

> The NEA is the highlight for most students. Start thinking about ideas now.

<!--
Mention that the NEA is entirely self-directed. They choose the problem,
they design the solution, they build it. It's the closest thing to real
professional software development they'll do at school.
-->

---

## The Bigger Picture

- A-Level CS opens doors to:
  - **University** — CS, Software Engineering, AI, Cyber Security …
  - **Apprenticeships** — degree apprenticeships at major tech companies
  - **Work** — the skills transfer to every career, not just tech

> Computational thinking is the skill of the century.

---

<!-- _class: section -->

# ☀️ Summer Preparation

*Totally optional — but genuinely rewarding.*

---

## Keep Learning Python

- Finish any GCSE Python topics you feel shaky on
- Start using **functions**, **classes** and **files** if you haven't
- Write at least one small project you care about

```python
# Example: a tiny habit tracker
habits = {}
habits["exercise"] = [True, False, True, True]
print(f"Completion: {sum(habits['exercise'])}/{len(habits['exercise'])}")
```

<!--
The goal isn't to rush ahead — it's to consolidate. Students who struggle
in Year 12 usually have gaps in the very basics: loops, functions, lists.
-->

---

## Read Tech News Regularly

| Publication | Best for |
|------------|---------|
| **The Register** | British tech industry news, witty writing |
| **Ars Technica** | In-depth technical journalism |
| **Hacker News** | Developer community links and discussion |
| **BBC Tech** | Accessible mainstream tech news |

> Reading widely makes the theory come alive — you'll recognise real examples in every topic.

---

## Follow Interesting Channels

| Channel | Why watch it |
|---------|-------------|
| **Computerphile** | CS theory explained brilliantly |
| **Fireship** | Fast, modern takes on languages and tools |
| **TechLinked** | Quick tech news roundup |
| **3Blue1Brown** | Maths and algorithms visualised |
| **NetworkChuck** | Networking and Linux hands-on |

> 10 minutes a day is all it takes.

<!--
Computerphile is especially relevant — many videos map directly to
topics in the spec. Recommend specific videos:
  - "Hashing Algorithms and Security"
  - "Floating Point Numbers"
  - "Huffman Encoding"
-->

---

## Complete a Free MOOC

<div class="columns">

**Top picks**
- **Harvard CS50** — the best intro CS course on the planet
- **Helsinki Python MOOC** — rigorous Python, free certificate
- **freeCodeCamp** — web, Python, data science tracks

**Also worth trying**
- Codecademy Python 3
- Kaggle Python (data focus)
- Automate the Boring Stuff

</div>

> CS50 alone will put you six months ahead. It's that good.

<!--
CS50 is at cs50.harvard.edu and is completely free. The first two weeks
cover C, which looks scary but teaches them about memory, pointers and
how Python actually works underneath.
-->

---

## Experiment with Linux

- Download **Ubuntu** or **Mint** — it's free
- Run it in a VM (VirtualBox) or on an old laptop
- Learn 10 terminal commands:

```bash
ls    cd    mkdir    rm    cp    mv
cat   grep  chmod    sudo
```

> A huge proportion of the world's servers run Linux. This is essential knowledge.

<!--
For students who are nervous, reassure them that Linux is just an
operating system. They can keep Windows and just try Linux in a VM.
The course covers operating systems in detail — this gives them a
head start.
-->

---

## Learn Basic Git and GitHub

```bash
# The three commands you use 90% of the time
git add .
git commit -m "Describe what you changed"
git push
```

1. Create a free account at **github.com**
2. Create a repository for your summer projects
3. Commit every time you make something work

> Your GitHub profile is your CV as a developer. Start it now.

<!--
Link them to the GitHub Student Developer Pack — it's free with a
school email and includes tonnes of useful tools.
-->

---

## Build Small Personal Projects

Ideas that are fun and educational:

- 🌡️ A weather script using a free API
- 📝 A flashcard quiz app (great for revision later!)
- 🎵 A script that renames your music files
- 📈 A stock price tracker
- 🎲 Any game you enjoy playing

> The best project is one you actually want to finish.

<!--
Emphasise: it doesn't matter if it's messy or unfinished. The point
is getting practice at starting, debugging, and iterating. That skill
is more valuable than any specific syntax.
-->

---

<!-- _class: section -->

# 📚 Recommended Resources

---

## Courses and Learning

| Resource | URL | Best for |
|----------|-----|---------|
| **Harvard CS50** | cs50.harvard.edu | Complete beginner-to-intermediate |
| **Helsinki Python MOOC** | mooc.fi/en | Rigorous Python with exercises |
| **freeCodeCamp** | freecodecamp.org | Broad tracks, project-based |
| **Real Python** | realpython.com | Practical Python tutorials |

> Most of these are completely free.

---

## YouTube Channels

| Channel | Focus |
|---------|-------|
| **Computerphile** | CS theory, security, algorithms |
| **Fireship** | Web, tools, modern dev culture |
| **TechLinked** | Weekly tech news |
| **3Blue1Brown** | Maths and visualisations |
| **NetworkChuck** | Linux, networking, hacking (ethical!) |

---

## News and Reading

| Site | Style |
|------|-------|
| **The Register** | register.co.uk — irreverent, British, excellent |
| **Ars Technica** | arstechnica.com — in-depth, trustworthy |
| **Hacker News** | news.ycombinator.com — links from practitioners |

> Start with one article a day. You'll be surprised how quickly it adds up.

<!--
Encourage students to bookmark these sites and spend 10 minutes in
the morning reading before school. It builds vocabulary, context and
genuine interest in the subject.
-->

---

<!-- _class: title -->

# Be curious.
# Build things.
# Break things.
# Learn how they work.

<!--
Leave this on screen while students pack up or during any Q&A.
This is the philosophy of the course in four lines.

If you want, ask the class: "What do you want to build this year?"
Take a few answers. Remember them — bring them up later in the year.
-->
