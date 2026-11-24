# Report Template

The report is two files.
`review.md` is what the student reads first and in full.
`corrections.md` is a worklist they tick off with the text open.
Keeping them apart is the point: a missing contribution statement must not sit in one list with a missing comma.

Number the findings so that the student can refer to them: S for structure, C for clarity, P for patterns, T for technical presentation, F for factual errors and contradictions.
Corrections are numbered per chapter.

Leave out a section only if it has no content, and say so in one line.

Every number in this template is a maximum, and zero is allowed.
A good text gets a short review: an area without problems gets one line that says so and is not filled with smaller points.

Headings in both files are in title case, as the rules require of the student's text.

## review.md

For a thesis, about 4,000 words is the ceiling, not counting the outline table; up to about 4,500 is fine.
It is not a target.
If the findings do not fit, shorten the minor ones; never drop a major one.

````markdown
# Review: <title>

<Thesis or paper; author if given>.
Reviewed on <date> from <files>, as <a final check | an early draft>.
This review covers how the text is written: structure, clarity, writing, and technical presentation.
It does not assess the research.

<For a PDF: "Page numbers are the ones printed on the pages.
In a PDF viewer that counts the pages of the file, add <k>.">

**In short:** <the verdict.
For each area (structure, clarity, writing, technical presentation), say whether it is fine or needs work, and where.
An area is fine if it has no major finding and no pattern of errors; minor findings and single corrections may remain.
For example: "The structure and the technical presentation are fine.
Clarity needs work in Chapter 3 (C1, C2).
The writing is fine; `corrections.md` lists 23 single corrections.">

## 1 How I Read Your <Thesis | Paper>

**Aim, as I understood it:** <one sentence>

**Contributions, as I understood them:**
1. <contribution>, supported in <chapter or section>
2. …

<Only if it applies: "If this is not what you meant, the text does not communicate it yet.
That is the first thing to fix.">

**From the introduction and conclusion alone,** an outsider learns <…>, but not <…>.

**What works:** <up to four specific points, each with the reason why it works>

**What does not work:** <up to four specific points about the text as a whole or about one of its main parts, such as the introduction or the evaluation; not about single places.
Each point says first what happens to a reader, then why, and names the finding that explains it: "At every 'node,' a reader has to work out whether a node of the control-flow graph or of the syntax tree is meant, because the word has two meanings (C1)."
This is the diagnosis; Section 2 turns it into steps.
If nothing fails at this level, write "Nothing at the level of the whole text." and add nothing.>

## 2 Fix These First

<At most five, the most important first.
Each is one sentence and points to the finding that explains it.>

1. **<short title>** (S1): <one sentence>
2. …

## 3 Structure

### 3.1 Outline, as I Read It

| Chapter | What it does | Supports contribution | Note |
|---|---|---|---|
| 1 Introduction | … | | … |

### 3.2 Major Findings

**S1 · <short title>** · <location>
*Rule:* <name (section)>.
<The rule in one sentence.>
*What a reader experiences:* <for example: "The reader reaches the formal definition in §3.2 without an example of what it should capture and has to read it twice.">
*How to fix it:* <the steps to take or the questions to answer, specific to this text.
Not the replacement text.>

### 3.3 Minor Findings

One line each, in reading order.

- **S6** · <location> · <rule name (section)>: <what is wrong and what to do, in one sentence>

## 4 Clarity and Accessibility

<Two or three sentences: who the readers of this text are (the table of readers in Section 1.1 of the structure rules), and how far each of them can follow it.>

### 4.1 Major Findings

**C1 · <short title>** · <location>
*Rule:* <name (section)>.
<The rule in one sentence.>
*What a reader experiences:* <which reader, and what happens to them.
For a concept with several names or a term with several meanings: every name or meaning in use, with its count and one location.>
*How to fix it:* <the steps to take.
For terminology: the one name you suggest, and what to check afterwards, such as the title.>

### 4.2 Minor Findings

One line each, in reading order.

- **C4** · <location> · <rule name (section)>: <what is wrong and what to do, in one sentence>

### 4.3 Where I Got Lost

Places where I stumbled as a first-time reader, in reading order.
Where a finding covers the place, name it.

- <location>: <what happened, in one line> <(C2)>

## 5 Writing: Patterns

`corrections.md` lists <n> single corrections and every instance of the patterns below.
Each pattern is explained once, here.

**P1 · <rule name (section), or a plain label where no rule states the case>** · <n> occurrences
*The rule:* <one or two sentences: what is right, and what a reader loses otherwise.
Under a plain label, head this line "The problem.">
*In your text:* "<original>" → "<corrected>" (<location>).
<One or two more.>
*Find the rest:* <a search or a check the student can run, for example: search for ", that">

<At most eight patterns, the most harmful first.
Further patterns go to corrections.md with their rule or label and their instances.>

## 6 Technical Presentation

### 6.1 Major Findings

**T1 · <short title>** · <location>
<In the three-part form of 3.2.>

### 6.2 Minor Findings

One line each, in reading order.

- **T2** · <location> · <rule name (section)>: <what is wrong and what to do, in one sentence>

## 7 Factual Errors and Contradictions

<Only the errors you are sure of.
One line each.>

- **F1** · <location>: "<original>".
  <The correct fact, and how to verify it.>

<Then one line: "<n> further places that may be wrong or that contradict each other are listed under 'Please Check' at the top of `corrections.md` (F<i> to F<j>)."
In an early draft, which has no corrections.md, list them here under a line "Please check:".>

## 8 Not Covered

<What you could not check: figures not visible in the source, a chapter that was not provided.
For an early draft: single language errors were not listed.
Then one line: the research itself is outside this review.>

The rule names refer to the guideline this review applies.
Ask for the full text of any rule.
````

## corrections.md

Written for a final check only.

````markdown
# Corrections: <title>

Reviewed on <date> from <files>.
<q> places to check, <m> patterns, and <n> corrections in <k> chapters.
Each row gives the location, the original, the correction, and the rule.
Patterns P1 to P<j> are explained in `review.md`.
<For a PDF: the same line on page numbers as in `review.md`.>

## Please Check

Places where the text may be wrong, or where two statements do not agree.
I am not sure of any of them, so check each one against your sources.

- **F9** · <location>: "<original>".
  <What does not fit, and what to compare it with.>

## Patterns: All Instances

**P1 · <rule name (section) or plain label>** · <n> instances
- `ch2.tex:14`: "<original>" → "<corrected>"
- `ch4.tex:31`: "<original>" → "<corrected>"
- "<original>" → "<corrected>": `ch2.tex:88`, `ch3.tex:9`, `ch5.tex:41` <identical instances share a line>

**P2 · <rule name (section)>** · <n> instances <a pattern of style>
<Locations, grouped by kind where that helps.>
Search for <what finds them>.

**P9 · <rule name (section) or plain label>** · <the rule or the problem in one sentence, because the review does not explain this pattern>
- `ch3.tex:40`: "<original>" → "<corrected>"

## Consistency Worklist

What the rules leave to the text, used in more than one form.
Each form has its count and one location.
Choose one form and search for the others.

- Compound that the dictionary does not list: "call graph" (14, p. 4), "callgraph" (3, p. 9), "call-graph" (1, p. 12) → "call graph"
- First person: "we" (41, p. 2), "I" (3, p. 12) → "we"

## Bibliography Worklist

Problems of the bibliography that cannot be given as a quotation and its replacement.
One line per entry or per kind of problem.

- Capitalization: acronyms in lowercase in four titles ("llvm", "ssa") → protect them with braces in the `.bib` file
- Pages: "page 12–20" in two entries, "pages" in the others → "pages"
- <Author (year)>: no venue → add it

## Chapter 1: <title>

| # | Location | Original | Correction | Rule |
|---|---|---|---|---|
| 1 | `intro.tex:12` | the set of variables are | the set of variables is | Agreement (2.3) |
| 2 | `intro.tex:31` | recieve | receive | spelling |

## Chapter 2: <title>

…
````

## Notes on the Entries

- **Location.**
  LaTeX and Markdown: `relative/path.tex:LINE`.
  PDF: `p. N, §X.Y`, with the number printed on the page, as the table of contents and the text's own references use it; the front matter keeps its roman numbers.
  Say once, near the top of each file, how the pages of the PDF file are counted against the printed numbers.
  Word: `§X.Y, ¶N`.
- **Original.**
  Verbatim, and the shortest fragment that a text search finds and that shows the error, usually three to eight words.
  Keep LaTeX markup that lies inside the fragment.
- **Correction.**
  The smallest change that repairs the error, written as the text that replaces the original, never as an instruction such as "delete X."
  The corrected text keeps to the rules itself.
  If two repairs are equally good, give both, separated by "/".
- **Rule.**
  The rule's exact name with its section number, but only if the text of the rule states the case.
  For any other error, write a plain label: "spelling," "grammar," "word choice," "punctuation," or the like.
  The same holds for the heading of a pattern.
- **Hints.**
  "How to fix it" and "Find the rest" name a command, a setting, or a search only if you are sure of its effect.
  Otherwise describe the result the student should reach.
- **One sentence, several errors.**
  One row with one corrected fragment; name the rules together.
- **A correction that belongs to a pattern** is listed under the pattern only, not again in the chapter table.
- **Instances of a pattern.**
  A pattern of errors (spelling, grammar, punctuation, usage) lists every instance with its location, original, and correction, because each instance needs its own fix.
  Identical instances share one line.
  A pattern of style lists its locations and the search that finds them.
  Every instance is a case that the text of the pattern's rule states.
  Instances that the rule does not state leave the pattern: three or more of one kind form a pattern of their own under a plain label, such as "grammar: singular for plural"; fewer go to the chapter tables with a plain label.
- **What a table of corrections holds.**
  Only rows with a verbatim original and the text that replaces it.
  A problem that needs a description, such as an incomplete bibliography entry or a technical compound in several forms, goes to the bibliography worklist or the consistency worklist.
- **Corrections.**
  A correction is an objective error, which a careful editor would not leave as it stands, or a departure from a rule of Sections 2.3 to 2.5.
  Where such a rule states the case, the rule decides.
  For any other error, the test is: could a careful native writer have written the original on purpose?
  If yes, it is not a correction.
  Single points of style that belong to no pattern are not listed; the student can ask for them.
- **Clarity findings.**
  Judge each against the reader of the part it stands in (the table of readers in Section 1.1 of the structure rules): an undefined term of the subfield is a finding in the introduction and in the main part of a thesis, and it is none in the related work of a paper.
  Terms and abbreviations that are used before they are defined, a concept with several names, a term with several meanings, a step that is left to the reader, and a formal statement without an example all belong here, not among the patterns.
  Pages that explain what the reader knows belong here too.
  The terms that the abstract, the introduction, or the conclusion uses without explaining them to an outside reader are one finding per part, which lists the terms.
- **Where the results of the consistency step go.**
  Names and meanings of terms: clarity findings.
  Clashing notation: findings on technical presentation.
  Statements that contradict each other: Section 7 or "Please Check."
  Departures from the rules of Section 2.5 on spelling, compounds, capitalization, and numbers: corrections, or a pattern where they recur.
  What the rules leave to the text, used in more than one form: the consistency worklist.
- **Certain and "please check."**
  A factual error is certain only if you are sure of the correct fact and can say how to verify it.
  Everything else is a place to check and goes to `corrections.md`.
  The two lists share one numbering, the certain ones first.
- **Major and minor.**
  A finding is major if a reader cannot follow or misses what the work contributes or how well it worked.
  Everything else that slows a reader in one place is minor.
  Do not promote a minor finding to make a section look weightier.
- **"Fix These First"** contains only major findings and certain factual errors.
  If there is no major finding, say so and name the two or three most useful minor ones.

## Follow-Up Review

Written instead of the first review when an earlier review exists (SKILL.md, "Follow-Up Review").
Both files get the date in their names, so that the earlier ones stay.
Number new findings on from the earlier review, so that no number means two things.

````markdown
# Follow-Up Review: <title>

Compared with the review of <earlier date>.
Reviewed on <date> from <files>.
This review checks what has changed since then.
It does not assess the research.

**In short:** <the verdict per area, as in the first review, and what is left.
If nothing is open and nothing new was found: "Nothing is open.
As far as this review goes, the text is ready.">

## 1 Earlier Findings

- **S1** <short title>: resolved.
- **C2** <short title>: partly resolved.
  <What is left, with locations.>
- **P2** <rule name (section)>: open, <k> of <n> instances left, listed in `corrections.md`.
- **C5** <short title>: withdrawn.
  <Why it did not hold, in one sentence.>
- Corrections: <a> of <b> done; the <c> open ones are listed in `corrections.md`.

## 2 New Findings

<Only objective errors and major findings on text that the earlier review saw, and any finding on text that was added or rewritten.
In the forms of the first review.
If there is none: "None.">

## 3 Not Covered

<As in the first review.>
````

The follow-up `corrections.md` lists the open corrections and pattern instances of the earlier review, with their earlier numbers, and then the new corrections, in the tables of the first review.
If nothing is open and nothing is new, it is not written; the review says so.
