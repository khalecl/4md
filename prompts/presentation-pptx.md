You are writing a Markdown file that the 4md tool converts into a designed PowerPoint deck (PPTX). The tool lays out each slide automatically, including SmartArt-style layouts, so your job is to write SLIDE TEXT, not prose. Write ONLY the Markdown file, inside one ```markdown code block, with no commentary.

TOPIC
[describe your topic, audience and length here]

HOW HEADINGS BECOME SLIDES
- `# Deck title` once, first line → cover slide. The single short line under it becomes the subtitle.
- `## Section name` with NOTHING under it before the next `###` → numbered section-divider slide.
- `### Slide title` → a content slide inside that section. (A `##` that has its own content is also a content slide.)
- `<!-- slide -->` on its own line → continue on a new slide with the same title.
- The tool adds an Agenda slide (from the sections) and a closing slide automatically — do not write them yourself.

SLIDE BUDGET (HARD LIMITS)
- One idea per slide. Slide titles ≤ 6 words, and they should state the point ("Controls deliver most savings"), not just a topic ("Controls").
- At most 6 bullets per slide, each ≤ 12 words. No full paragraphs; at most one sentence of plain text per slide.
- Put detail, explanations and examples in speaker notes: `<!-- notes: what the presenter should say -->` (one line, directly under the slide content).

SMART LAYOUTS — write the list in the matching shape and the tool draws it
| Write this | You get |
|---|---|
| `- **Term**: short description` (2–6 items) | Cards with headings |
| `1. Short step` (2–5 items, ≤ 6 words each) | Process chevrons |
| `1. Longer step sentence` (2–6 items) | Numbered vertical steps |
| `- Q1: …`, `- 2026: …`, `- Phase 1: …`, `- Week 2: …` (2–6 items) | Timeline |
| `- **42%**: what the number means` (2–6 items) | Big-number stat tiles |
| 2–4 short top items each with indented `- ` sub-bullets | Coloured columns (good for compare/contrast) |
| 2–6 short plain bullets | Numbered tiles |

Force a layout by putting a directive on the line BEFORE the list:
`<!-- layout: cards -->` — choices: cards, tiles, process, steps, timeline, columns, stats, bullets (bullets = plain list).

OTHER SLIDE ELEMENTS
- Tables: pipe tables, ≤ 5 columns, ≤ 6 rows; right-align numbers with `---:`. Longer tables continue on "(cont.)" slides — avoid that.
- Diagrams: ```mermaid fenced blocks (flowchart LR/TD, pie, timeline, mindmap, gantt). ≤ 8 nodes. A diagram plus ≤ 3 bullets sits side by side.
- Equations: display maths between `$$ … $$` on its own lines; inline `$…$` is shown as plain symbols.
- A single `> quote` line becomes a highlighted callout slide element — use for a strong key message.
- Code: short fenced blocks (≤ 12 lines) only when the audience is technical.

DO NOT USE
Raw HTML (other than the comment directives above), images, links as content, paragraphs over 25 words, more than 2 elements on one slide.

PACE
Aim for roughly one content slide per 2 minutes of talk. Mix layouts — never more than two plain-bullet slides in a row. Close with a `## Key Takeaways` slide written as `- **Term**: …` cards or `- **number**: …` stats.
