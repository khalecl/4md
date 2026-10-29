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
| `# Title` + one line | Cover slide |
| `## Section` with no content before its `###` | Numbered section divider |
| `### Title` | Content slide |
| `- **Term**: description` | Cards |
| `1. Short step` | Process chevrons |
| `1. Longer step sentence` | Vertical steps |
| `- Q1: …` / `- 2026: …` / `- Phase 1: …` | Timeline |
| `- **42%**: meaning` | Big-number stat tiles |
| Short items with sub-bullets | Columns |
| Short plain bullets | Numbered tiles |

### Deck-only directives (invisible in DOCX/PDF)

```markdown
<!-- layout: cards -->        force the next list's layout (cards, tiles, process, steps, timeline, columns, stats, bullets)
<!-- notes: presenter text --> speaker notes
<!-- slide -->                 new slide, same title
<!-- slide-only --> … <!-- /slide-only -->   content only in the deck
<!-- doc-only -->   … <!-- /doc-only -->     content only in DOCX/PDF
```

## AI prompts

Press **🤖 AI Prompt** in the app, or use the files in [`prompts/`](prompts):

- [`document-docx-pdf.md`](prompts/document-docx-pdf.md): reports, manuals and handouts
- [`presentation-pptx.md`](prompts/presentation-pptx.md): slide decks
- [`document-and-deck.md`](prompts/document-and-deck.md): one file that makes both

## Examples

- [`examples/smart-layouts-demo.md`](examples/smart-layouts-demo.md): one slide per layout
- [`examples/document-and-deck.md`](examples/document-and-deck.md): doc-only / slide-only / notes in action

## Built with

Marked, JSZip, KaTeX, Mermaid, html2canvas, html2pdf.js and PptxGenJS, all loaded from CDNs. Settings and templates are saved in your browser.
