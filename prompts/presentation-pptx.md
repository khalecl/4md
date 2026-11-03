You will write a PowerPoint deck as Markdown. A tool called 4md turns your Markdown into designed slides, so you only write the text, in the exact format below.

TOPIC
[describe your topic, audience and length here]

OUTPUT
Reply with the Markdown only: no greeting, no explanation and no code fence around it. Start your reply with the line that begins with "# ".

HOW TO BUILD THE DECK, STEP BY STEP
1. Line 1: `# Deck title`. Line 2: one short subtitle sentence.
2. Plan 3 to 5 sections. Start each one with `## Section name` and put nothing under that heading; it becomes a divider slide.
3. Under each section write 2 to 4 slides. Each slide starts with `### Slide title`. A slide title is a short statement of the point, 3 to 7 words, for example "Controls deliver most savings", not "Controls".
4. Each slide has ONE content block, chosen from the list below. Use a different block type from the slide before it.
5. Each slide ends with a speaker-notes line (rules below). EVERY `###` slide needs one.
6. Finish with `## Key Takeaways` followed directly by 3 or 4 `- **Term**: text` lines and a notes line.
Do not write an Agenda slide or a Thank-you slide; the tool adds both.

CONTENT BLOCKS (use the exact shapes shown)
A. Cards, 3 or 4 items:
- **Short heading**: one line of explanation
B. Process, 3 to 5 steps:
1. **Step name**: what happens
C. Big numbers, 2 to 4 items (percentages draw as rings):
- **61%**: what the number means
D. Timeline, 3 to 5 items:
- Q1: what happens
(other labels that work: 2026:, Phase 1:, Week 1:, Month 1:)
E. Comparison columns, 2 or 3 headings with 2 or 3 indented points each:
- Option A
    - point
    - point
- Option B
    - point
    - point
F. Chart: a line `<!-- chart: bar -->` (or line, pie, doughnut), then a table whose first column holds labels and whose other columns hold numbers:
<!-- chart: bar -->
| Item | Value |
|:---|---:|
| First | 120 |
| Second | 340 |
G. Statement: one short, strong sentence on its own (it becomes a full-colour slide). Use 1 or 2 per deck.
H. Quote: `> The quote text. — Real source`. Use it only for a real, attributable quote.
I. Simple list: 3 to 5 `- ` bullets, at most 10 words each.

SPEAKER NOTES (required on every ### slide)
- Write them on ONE line, directly under the slide's content, in exactly this form:
<!-- notes: What the presenter says out loud on this slide. -->
- Write 3 to 5 full sentences of spoken script, in the first person, as the presenter will actually say them. Explain the point, give one example, fact or figure that is not already on the slide, and end with a sentence that leads into the next slide.
- Do not just repeat the bullets, and do not describe the slide ("This slide shows…").

LIMITS
- At most 6 items per list and at most 12 words per item.
- Keep numbers, units and standard names as they are written (kWh, ISO 50001).
- Mark any estimated figure "(est.)". Never invent statistics or quotes and present them as fact.
- No HTML except the `<!-- notes: … -->` and `<!-- chart: … -->` lines, and no images unless asked.
- Write in the language of the topic. Arabic, Hebrew, Persian and Urdu decks are mirrored right-to-left automatically.

COMPLETE EXAMPLE (copy this structure exactly, not the content)
# Energy Audit Programme 2026
Cutting energy cost and carbon across our buildings

## Why We Are Auditing

### Energy is our largest controllable cost
- **32%**: of operating spend goes on electricity
- **61%**: of that electricity is used for cooling
- **18%**: typical saving found by a first audit
<!-- notes: I want to start with the size of the problem. Almost a third of what we spend to run our buildings goes on electricity, and most of it is cooling. That matters because cooling is also where controls make the biggest difference. In a typical first audit we find savings close to one fifth, so let us look at why now is the right time to act. -->

### Four reasons to act now
- **Cost**: tariffs rose twice in two years
- **Compliance**: ISO 50001 certification is due next year
- **Carbon**: Scope 2 cuts are needed for the ESG report
- **Reliability**: old chillers fail more often
<!-- notes: There are four separate pressures, and any one of them would justify this work. The tariff increases alone added to our bill last year. Certification and the ESG report both need measured data, which the audit will give us. And older chillers break down more, so finding problems early protects our operations as well as our budget. -->

### Most savings come from controls
Most savings come from controls, not new equipment.
<!-- notes: If you remember one thing from today, make it this. Changing schedules, setpoints and the order in which chillers start costs very little. New equipment comes later, once we know exactly where the energy goes. Next, I will show you how the audit finds those opportunities. -->

## How The Audit Works

### Five steps over twelve weeks
1. **Scope**: agree sites and data access
2. **Measure**: install loggers on main loads
3. **Survey**: walk through every plant room
4. **Analyse**: build the baseline and savings model
5. **Report**: costed measures and a verification plan
<!-- notes: The audit runs in five steps over about twelve weeks. Measuring and surveying overlap, because the loggers need at least two weeks of data before the analysis starts. The report gives each measure a cost and a payback, so decisions are easy. Let me show you where we expect those savings to come from. -->

### Savings build through the year
<!-- chart: bar -->
| Quarter | Savings (MWh, est.) |
|:---|---:|
| Q1 | 120 |
| Q2 | 410 |
| Q3 | 690 |
| Q4 | 860 |
<!-- notes: These figures are estimates from similar sites. Savings start small while we install metering, then grow quickly once the quick wins are in place. By the fourth quarter we expect around eight hundred and sixty megawatt-hours. That brings me to the main points to take away. -->

## Key Takeaways
- **Controls first**: the cheapest savings come before any capital spend
- **Meter everything**: no data, no decisions
- **Verify**: report savings with an agreed method
<!-- notes: To close, three points. Start with controls, because they pay back fastest. Measure everything, because every later decision depends on data. And verify the savings in a way finance agrees with, so the results are trusted. I am happy to take your questions. -->

FINAL CHECK BEFORE YOU REPLY
- The first line starts with "# ", and there is no code fence anywhere around the deck.
- Every `###` slide has exactly one content block and one `<!-- notes: … -->` line of 3 to 5 spoken sentences.
- Consecutive slides use different block types, and there is at least one chart or big-numbers slide.
- There is no Agenda slide and no Thank-you slide.
