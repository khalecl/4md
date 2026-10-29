# 4md

**Markdown → Word, PDF and PowerPoint, in one browser page.**

4md is a single self-contained HTML file. Open `index.html` in a browser (or via GitHub Pages), paste or load a `.md` file, and download:

| Output | What you get |
|---|---|
| **DOCX** | Real Word styles (Title, Heading 1–4, Quote, Code, Table), templates, page layout, header/footer, document properties |
| **PDF** | The same template rendered to PDF: fonts, margins, header/footer, page numbers |
| **PPTX** | A designed deck: 16 themes, cover, agenda, section dividers, SmartArt-style layouts, speaker notes, closing slide |

## Supported markdown

Headings, **bold**/*italic*, nested lists, pipe tables with alignment, quotes, fenced code, KaTeX maths (`$…$`, `$$…$$`), Mermaid diagrams, and `::indent:N::` indented paragraphs.

## Slides: how markdown becomes a deck

| Markdown | Slide |
|---|---|
| `# Title` + one line | Cover slide (split, full colour, band or centred) |
| `## Section` with no content before its `###` | Numbered section divider; the Agenda slide is built from these |
| `### Title` | Content slide (content is centred vertically) |
| `- **Term**: description` | Cards with automatic icons |
| `1. **Step**: description` | Process chevrons |
| `1. Longer step sentence` | Numbered vertical steps |
| `- Q1: …` / `- 2026: …` / `- Phase 1: …` | Timeline |
| `- **42%**: meaning` | Ring charts (percentages) or big-number tiles |
| Short items with sub-bullets | Columns |
| Short plain bullets | Icon tiles |
| One short sentence, one `> quote — source`, or one stat alone | Full-colour statement slide |
| `<!-- chart: bar -->` above a table | Native, editable chart (bar, hbar, line, area, pie, doughnut, radar) |
| `![caption](url)` or `![caption]()` | Picture beside the text, or a picture placeholder |
| ```` ```mermaid ```` | Diagram beside the text |

### Deck-only directives (invisible in DOCX/PDF)

```markdown
<!-- layout: cards -->         force the next list's layout (cards, icons, process, steps, timeline, columns, stats, statement, bullets)
<!-- chart: bar -->            turn the next table into a chart
<!-- icons: bolt, money, leaf --> choose the icons for the next list
<!-- notes: presenter text -->  speaker notes
<!-- slide -->                  new slide, same title
<!-- slide-only --> … <!-- /slide-only -->   content only in the deck
<!-- doc-only -->   … <!-- /doc-only -->     content only in DOCX/PDF
```

Icons: bolt money clock check users leaf gauge shield chart gear building drop sun thermo target bulb doc flag search alert factory plug wrench globe rocket calendar trend image cloud star book truck lock handshake.

### Slide settings (Settings → Slides)

- **16 themes**, plus **your own**: load any `.pptx` / `.potx` / `.thmx` and its colours, fonts and slide size become the ★ My template theme.
- **Style**: title style, cover style, card style (soft, shadow, outline, solid), decoration (circles, dots, stripes, blocks), text size (large / standard / compact), bullet marker, fonts.
- **Content**: smart layouts on/off, icons, ring charts, vertical centring, slide transitions (fade, push, wipe, cover, split).
- **Deck**: aspect ratio, agenda, closing slide and text, slide numbers, footer, cover details, **logo**.
- **Check my deck**: flags long titles, crowded slides, wordy bullets, big tables, missing notes and repeated plain-bullet slides before you export.
- **Analyze a .pptx**: reports words per slide, font sizes, visuals and notes for any deck, takes its colours and fonts, or loads its text as markdown so you can restyle it here.

## AI prompts

Press **🤖 AI Prompt** in the app, or use the files in [`prompts/`](prompts):

- [`document-docx-pdf.md`](prompts/document-docx-pdf.md): reports, manuals and handouts
- [`presentation-pptx.md`](prompts/presentation-pptx.md): slide decks
- [`document-and-deck.md`](prompts/document-and-deck.md): one file that makes both

## Examples

- [`examples/smart-layouts-demo.md`](examples/smart-layouts-demo.md): one slide per layout
- [`examples/document-and-deck.md`](examples/document-and-deck.md): doc-only / slide-only / notes in action
- [`examples/energy-audit-deck.md`](examples/energy-audit-deck.md): a complete 10-slide presentation using every slide feature
- [`examples/chiller-plant-deck.md`](examples/chiller-plant-deck.md): pictures, charts, a diagram and a big-number slide

## Built with

Marked, JSZip, KaTeX, Mermaid, html2canvas, html2pdf.js and PptxGenJS, all loaded from CDNs. Settings and templates are saved in your browser.
