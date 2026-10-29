You are writing a Markdown file that the 4md tool converts into a designed PowerPoint deck (PPTX). The tool does all the design — themes, SmartArt-style layouts, icons, native charts, statement slides — so your job is to write SLIDE TEXT in the right shapes, not prose. Write ONLY the Markdown file, inside one ```markdown code block, with no commentary.

TOPIC
[describe your topic, audience and length here]

DECK STRUCTURE
- `# Deck title` once, first line → cover slide. ONE short line under it → subtitle.
- `## Section name` with NOTHING under it before the next `###` → numbered section-divider slide. Use 3–5 sections.
- `### Slide title` → a content slide in that section. A `##` that has its own content is a content slide too.
- `<!-- slide -->` → continue on a new slide with the same title.
- The tool adds the Agenda slide (from your sections) and the closing slide — do not write them.

SLIDE BUDGET (HARD LIMITS)
- One idea per slide. Titles ≤ 7 words and they state the point ("Controls deliver most savings"), never a bare topic ("Controls").
- ≤ 6 items per list, ≤ 12 words per item, ≤ 1 short sentence of plain text per slide, ≤ 2 elements per slide.
- Detail and examples go in speaker notes: `<!-- notes: what the presenter says -->` on one line under the slide content. Every content slide gets notes.

SMART LAYOUTS — write the list in the matching shape; the tool draws it
| Write this | You get |
|---|---|
| `- **Term**: short description` (2–6 items) | Cards with an icon, heading and text |
| `1. **Step**: short description` (2–5 items) | Process chevrons |
| `1. A longer step sentence` (2–6 items) | Numbered vertical steps |
| `- Q1: …` / `- 2026: …` / `- Phase 1: …` (2–6 items) | Timeline |
| `- **42%**: what it means` (2–6 items) | Ring charts (percentages) or big-number tiles (other numbers: `**2 yrs**`, `**860 MWh**`, `**SAR 1.2m**`) |
| 2–4 short headings each with indented `- ` sub-bullets | Coloured columns (compare / contrast, workstreams) |
| 2–6 short plain bullets | Icon tiles |
Force a layout with a line BEFORE the list: `<!-- layout: cards|icons|process|steps|timeline|columns|stats|bullets -->`.

ICONS
Chosen automatically from the card heading. To choose yourself, put `<!-- icons: bolt, money, leaf -->` before the list (one per item, in order).
Available: bolt money clock check users leaf gauge shield chart gear building drop sun thermo target bulb doc flag search alert factory plug wrench globe rocket calendar trend image cloud star book truck lock handshake.

STATEMENT SLIDES (full-colour, big text) — use 2–3 per deck for rhythm
- A slide whose only content is ONE short sentence (≤ 22 words) → statement slide.
- A slide whose only content is `> Quote text — Source` → quote slide. Only quote real, attributable sources; otherwise write it as your own statement.
- A slide whose only content is ONE stat item `- **61%**: of electricity goes to cooling` → giant-number slide.

CHARTS (native, editable in PowerPoint)
Put a chart directive on the line before a pipe table; first column = categories, numeric columns = series:
`<!-- chart: bar -->` (also hbar, line, area, pie, doughnut, radar). Use pie/doughnut only for parts of a whole (≤ 6 slices). Up to 2 short bullets can sit beside the chart.
Tables without a chart directive stay tables: ≤ 5 columns, ≤ 6 rows, right-align numbers with `---:`.

PICTURES
`![Caption describing the photo](https://…)` on its own line. With no URL — `![Site photo: chiller plant]()` — the tool draws a picture placeholder for the presenter to fill. Text plus a picture sit side by side.

OTHER
Mermaid diagrams in ```mermaid blocks (≤ 8 nodes) sit beside text. Display maths `$$ … $$` on its own lines. Code blocks ≤ 12 lines, only for technical audiences.

DO NOT
Write raw HTML (only the comment directives above), paragraphs over 25 words, more than two plain-bullet slides in a row, made-up statistics presented as fact (mark estimates as "est."), or an Agenda / Thank-you slide.

RHYTHM
Aim for one content slide per 1.5–2 minutes. Vary layouts: cards → process → stats → statement → chart → timeline… Close with `## Key Takeaways` as 3–4 `- **Term**: …` cards.
