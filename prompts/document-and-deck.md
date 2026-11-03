You are writing ONE Markdown file that the 4md tool converts into BOTH a professional Word/PDF document AND a designed PowerPoint deck. HTML comments steer the deck and are invisible in the document. Reply with the Markdown only: no commentary and no code fence around it. Start with the line that begins with "# ".

TOPIC
[describe your topic, audience and length here]

THE TWO-AUDIENCE RULE
- Text that both outputs should show: write normally.
- Detail for the document only (explanatory paragraphs, long tables, references): wrap it in
  <!-- doc-only -->
  …markdown…
  <!-- /doc-only -->
- Short slide text the document does not need (punchy bullets, stat tiles): wrap it in
  <!-- slide-only -->
  …markdown…
  <!-- /slide-only -->
- Presenter script: `<!-- notes: … -->` on one line (deck only).
- Force a slide layout for the next list: `<!-- layout: cards|tiles|process|steps|timeline|columns|stats|bullets -->`.
- `<!-- slide -->` starts a new slide with the same title (deck only).

HEADINGS
- `# Title` once (cover slide + document title); one short subtitle line under it.
- `## Section` → document section; in the deck, a numbered divider slide when it has no content of its own before its `###` slides.
- `### Topic` → document sub-section; one deck slide each. Titles ≤ 6 words and state the point.

FOR EACH ### TOPIC USE THIS PATTERN
1. A slide-ready list (≤ 6 items, ≤ 12 words each) written in a smart-layout shape:
   - `- **Term**: description` → cards
   - `1. Short step` → process chevrons; `1. Longer step` → vertical steps
   - `- Q1: …` / `- 2026: …` / `- Phase 1: …` → timeline
   - `- **35%**: meaning` → stat tiles
   - 2–4 short items each with indented sub-bullets → columns
   - `- **61%**: meaning` alone on a slide → giant-number slide; one short sentence alone → statement slide
   - `<!-- chart: bar|line|pie|doughnut -->` above a numeric table → native chart in the deck; the document still shows it as a normal table
   - `![Caption]()` → picture placeholder beside the text
2. A speaker-notes line, on ONE line and REQUIRED on every `###` slide: `<!-- notes: … -->`. It holds 3 to 5 full sentences of what the presenter says out loud, in the first person, adding an example or fact that is not on the slide and leading into the next slide. Do not repeat the bullets.
3. A `<!-- doc-only -->` block with the full explanation: paragraphs, worked examples, tables and equations.

SUPPORTED MARKDOWN (both outputs)
**bold**, *italic*, `code`; nested lists (4-space indent); pipe tables with alignment (`:---`, `:---:`, `---:`), same cell count in every row; `> quote`; fenced code with a language; KaTeX maths `$inline$` and `$$display$$` on their own lines (escape `\$`); ```mermaid diagrams (≤ 8 nodes on slides, quote labels with spaces/symbols); `::indent:1::` indented paragraph (document only); `---` rule.

LANGUAGE
Write in the language of the topic. Arabic, Hebrew, Persian and Urdu decks are detected automatically and the whole deck is mirrored right-to-left; keep numbers, units and standard names (ISO 50001, kWh) in Latin script.

DO NOT USE
Raw HTML other than the directives above, images, footnotes, setext headings, or numbers typed into headings.

FINISH WITH
`## Key Takeaways` — a `- **Term**: …` or `- **number**: …` list (slides) followed by a short doc-only summary paragraph.
