You are writing a Markdown file that will be converted into a professional Word document (DOCX) and PDF by a tool called 4md. Write ONLY the Markdown file, inside one ```markdown code block, with no commentary before or after.

TOPIC
[describe your topic, audience and length here]

STRUCTURE
- `# Title` exactly once, on the first line. The paragraph right under it is the document subtitle / summary.
- `## Section`, `### Sub-section`, `#### Minor heading`. Never skip a level (no ### directly under #).
- Keep paragraphs short (2–5 sentences). One idea per paragraph.

FORMATTING THE TOOL SUPPORTS — USE THEM WHERE THEY HELP
- Inline: **bold**, *italic*, ***bold italic***, `inline code`.
- Bullet lists with `- `; numbered lists with `1. `. Nest by indenting 4 spaces (up to 3 levels).
- Indented paragraph without a bullet: start the line with `::indent:1::` or `::indent:2::`.
- Tables: GitHub pipe tables with a header row and a separator row. Set alignment in the separator: `:---` left, `:---:` centre, `---:` right. Right-align numbers. Every row must have the same number of `|` cells; leave a cell empty rather than dropping it. Keep tables to 7 columns or fewer.
- Block quotes: lines starting with `> ` — use for key takeaways, definitions or cited statements.
- Code: fenced blocks with a language, e.g. ```python. Keep lines under 90 characters.
- Equations (KaTeX/LaTeX): inline `$E = P \times t$`; display equations on their own lines between `$$` and `$$`. Escape a literal dollar sign as `\$`.
- Diagrams: fenced ```mermaid blocks (flowchart TD/LR, sequenceDiagram, gantt, pie, classDiagram, stateDiagram-v2, mindmap, timeline). Keep node labels short; wrap labels with spaces or special characters in double quotes: A["Chiller (500 kW)"]. No HTML inside Mermaid labels.
- Horizontal rule `---` on its own line for a visual break.

DO NOT USE
- Raw HTML, images, footnotes, emoji-heavy text, `<br>`, setext headings (=== / ---) or tables inside lists.
- Hard-coded numbering in headings ("1.2 Scope") — the template styles headings.

QUALITY
- Write for a professional reader. Be specific: real figures, units (kW, kWh, °C, SAR) and standards where relevant.
- Every table and diagram gets a one-sentence lead-in paragraph before it that says what it shows.
- End with a `## Summary` or `## Key Takeaways` section.
