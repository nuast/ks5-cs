# KS5 Computer Science — OCR A-Level (H446)

> Teaching materials for OCR A-Level Computer Science (Years 12–13).  
> All presentations are written in **Marp** Markdown and organised by topic.

---

## 📂 Repository Structure

```
ks5-cs/
│
├── assets/                   ← Shared media
│   ├── images/               ← Photos, screenshots
│   ├── diagrams/             ← Technical diagrams (SVG, PNG)
│   └── logos/                ← School / OCR logos
│
├── themes/
│   └── ks5.css               ← Custom Marp theme (dark, modern)
│
├── templates/
│   ├── lesson.md             ← Starting point for a new lesson deck
│   └── title.md              ← Unit title slide
│
├── 00-Introduction/          ← Transition, induction and course overview
├── 01-Programming/           ← Python, OOP, paradigms
├── 02-Algorithms/            ← Searching, sorting, complexity
├── 03-Data/                  ← Data types, structures, representation
├── 04-Computer-Systems/      ← Processors, memory, OS, software
├── 05-Networking/            ← Protocols, hardware, security
├── 06-Cyber-Security/        ← Threats, defences, legislation
├── 07-Databases/             ← SQL, normalisation, transactions
├── 08-Functional-Programming/← Haskell / functional concepts
├── 09-Theory/                ← Boolean algebra, Turing machines, languages
├── 10-NEA/                   ← Programming project guidance
│
├── extras/                   ← Enrichment, careers, trips
│
├── computer-systems/         ← Existing revision notes (spec-aligned)
├── algorithms-programming/   ← Existing revision notes (spec-aligned)
├── programming-project/      ← Existing NEA guidance
│
└── README.md
```

The numbered topic folders (`01-Programming/` etc.) are for **Marp slide decks**.  
The lettered folders (`computer-systems/`, `algorithms-programming/`) are legacy **revision notes**.

---

## 🛠️ Editing Presentations

### Prerequisites

Install the Marp CLI (requires Node.js):

```bash
npm install -g @marp-team/marp-cli
```

Or use the **Marp for VS Code** extension (recommended for day-to-day editing):

1. Open VS Code.
2. Install the extension: `Marp Team — Marp for VS Code`.
3. Open any `.md` file with `marp: true` in the front-matter.
4. Click the **preview** icon (top-right) or press `Ctrl+Shift+P → Marp: Open Preview`.

### Registering the custom theme

Add the theme path to VS Code settings (`.vscode/settings.json`):

```json
{
  "markdown.marp.themes": [
    "./themes/ks5.css"
  ]
}
```

Then set `theme: ks5` in a slide deck's front-matter.

---

## 👁️ Previewing Slides

**VS Code (recommended)**

Open the file and use the Marp preview pane. Changes appear live.

**Browser preview via CLI**

```bash
marp --watch --theme themes/ks5.css 00-Introduction/year11-to-year12-transition.md
```

This opens a local server and reloads the preview whenever you save.

---

## 📤 Exporting Presentations

### HTML (self-contained — easy to share)

```bash
marp --html --theme themes/ks5.css path/to/deck.md -o path/to/deck.html
```

### PDF

```bash
marp --pdf --theme themes/ks5.css path/to/deck.md -o path/to/deck.pdf
```

### PowerPoint (PPTX)

```bash
marp --pptx --theme themes/ks5.css path/to/deck.md -o path/to/deck.pptx
```

### Export all decks at once

```bash
# HTML — every .md file with marp: true
marp --html --theme themes/ks5.css --input-dir . --output _exports/
```

---

## 🆕 Creating a New Presentation

1. **Copy a template:**

   ```bash
   cp templates/lesson.md 01-Programming/variables-and-types.md
   ```

2. **Edit the front-matter** — update `header`, `footer`, and the title slide.

3. **Add slides** — one idea per slide. Use `---` to separate slides.

4. **Use the theme classes** where needed:

   | Class | Usage |
   |-------|-------|
   | `<!-- _class: title -->` | Title / cover slide |
   | `<!-- _class: section -->` | Section divider |
   | `<!-- _class: invert -->` | Light background slide |

5. **Add presenter notes** inside `<!-- ... -->` HTML comments.

---

## 🎨 Theme Reference (`themes/ks5.css`)

### Colours

| Role | Value |
|------|-------|
| Background | `#1a1a2e` deep navy |
| Accent / headings | `#e94560` coral-red |
| Code background | `#0d1117` GitHub dark |
| Surface (invert bg) | `#f0f2f5` near-white |

### Two-column layout

```html
<div class="columns">

Left column content here.

Right column content here.

</div>
```

### Badge / inline label

```html
Some text <span class="badge">NEW</span>
```

---

## 📝 Marp Front-Matter Reference

```yaml
---
marp: true          # required — enables Marp
theme: ks5          # our custom theme
paginate: true      # slide numbers
header: "H446 · Topic Name"
footer: "© 2025 — Your Name"
---
```

---

## 🖼️ Using Images

**Background image (right-aligned, takes 40% of width):**

```markdown
![bg right:40%](../assets/images/your-image.png)
```

**Centred image:**

```markdown
![center width:500px](../assets/diagrams/your-diagram.svg)
```

**Full-bleed background with dim:**

```markdown
![bg opacity:0.3](../assets/images/your-image.jpg)
```

---

## 📋 Topic Index

| Folder | OCR Component | Topics |
|--------|--------------|--------|
| [00-Introduction](00-Introduction/) | — | Transition, induction, course overview |
| [01-Programming](01-Programming/) | 02 | Python, OOP, paradigms |
| [02-Algorithms](02-Algorithms/) | 02 | Searching, sorting, complexity |
| [03-Data](03-Data/) | 01 | Data types, structures, representation |
| [04-Computer-Systems](04-Computer-Systems/) | 01 | Processors, memory, OS, software |
| [05-Networking](05-Networking/) | 01 | Protocols, hardware, the internet |
| [06-Cyber-Security](06-Cyber-Security/) | 01 | Threats, defences, legislation |
| [07-Databases](07-Databases/) | 01 | SQL, normalisation, transactions |
| [08-Functional-Programming](08-Functional-Programming/) | 02 | Functional concepts, Haskell |
| [09-Theory](09-Theory/) | 01/02 | Boolean algebra, automata, languages |
| [10-NEA](10-NEA/) | 03 | Programming project guidance |

---

## 🔗 Useful Links

- [Marp documentation](https://marpit.marp.app/)
- [Marp CLI reference](https://github.com/marp-team/marp-cli)
- [Marp for VS Code](https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode)
- [OCR H446 specification](https://www.ocr.org.uk/Images/170844-specification-accredited-a-level-gce-computer-science-h446.pdf)

---

*Materials aligned to OCR A-Level Computer Science specification H446. Not an OCR official publication.*
