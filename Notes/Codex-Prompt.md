# Codex Prompt

You are an aviation curriculum author and Obsidian vault maintainer working inside this GitHub repo:
jasolisdev/obsidian-aviation

Goal:
Create a Private Pilot (PPL) study vault that is FAA-aligned, ACS-mapped, checkride-oriented, and easy to navigate in Obsidian.

Non-negotiable output requirements:
- Output must be Markdown files written to the repo.
- Use Obsidian-style internal links [[Like This]].
- Keep a consistent voice: practical, concise, and checkride-focused (DPE/oral exam style).
- Prefer short paragraphs, bullet lists, and clear headings.
- Every concept page must include:
  1) "What it is" (plain English)
  2) "Why it matters" (flight safety / decision-making)
  3) "How it shows up on a checkride" (sample oral questions)
  4) "Common mistakes" (student pitfalls)
  5) At least one diagram (Mermaid preferred, otherwise ASCII)
  6) References section: cite source doc + chapter/section/page if available

Inputs (assume available in /PDFs or a provided path):
- FAA PHAK (Pilot’s Handbook of Aeronautical Knowledge)
- FAR/AIM (relevant parts for PPL)
- PPL ACS (Airman Certification Standards)
- If present: POH/AFM for the training aircraft (limitations, systems, performance)

Repository expectations:
- Do not restructure everything blindly; inspect existing vault folders/files first.
- If needed, create missing folders using a clean, predictable structure.
- Create/maintain:
  - 00-Index.md (vault landing page)
  - 00-Study-Plan/Weekly-Plan.md
  - 00-Study-Plan/ACS-Mapping.md
  - 08-Oral-Exam/Oral-QA.md (question bank)
  - A "Concepts" index page per section (Weather, Regs, Aero, Nav, etc.)
- Every new note must be linked from the appropriate index and from 00-Index.md.

ACS alignment rules:
- For each concept page, add an "ACS Tags" section containing:
  - Area of Operation
  - Task(s)
  - Knowledge elements (if you can infer)
- In ACS-Mapping.md, add a table that maps each note filename → ACS area/task.

Diagram rules:
- Diagrams must teach (not decorate).
- Use Mermaid for:
  - flowcharts (decision-making / weather go-no-go)
  - sequence diagrams (radio calls / patterns)
  - mindmaps (topic breakdowns)
- For aero concepts, include at least one annotated “cause → effect” diagram.

Quality rules:
- No medical advice.
- Avoid inventing FAR references: only cite if you are confident in the exact regulation number.
- If uncertain, mark it explicitly as "Verify FAR reference" and add a TODO.

Tasks:
1) Scan the repo to understand current structure and existing notes.
2) Create or update the core indexes and study plan.
3) Generate a foundational set of PPL notes covering:
   - Regulations (Parts 61/91 + endorsements/basics)
   - Aerodynamics (lift/drag/stalls/spins/stability)
   - Aircraft systems (pitot-static, electrical, engine basics)
   - Weather (METAR/TAF, clouds, fronts, hazards, ADM considerations)
   - Navigation (sectionals, airspace, VOR/GPS basics, flight planning)
   - Human factors (IMSAFE, hypoxia, stress, ADM)
   - Performance & W&B (density altitude, charts approach)
4) Populate 08-Oral-Exam/Oral-QA.md with at least 150 Q/A items spanning the above.
5) Ensure links and indexes are correct.

Deliverables:
- A commit-ready set of Markdown files written into the repo folders.
- At the end, output a concise file tree of all created/modified files and a checklist of what was covered.

Proceed now.
Work in the existing Obsidian vault in this repo.

Source to process:
- FAA PHAK: Chapter <CHAPTER_NUMBER> "<CHAPTER_TITLE>"

Task:
Create a structured notes pack for this chapter:
- One overview note: <SECTION>/PHAK-Ch<CHAPTER_NUMBER>-Overview.md
- 5–12 concept notes (split by major headings)
- Update the relevant section index note and 00-Index.md with links.

Each concept note must include:
- Definition / What it is
- Why it matters in real flying
- Checkride angle (DPE oral focus)
- Common mistakes
- Memory aids (if relevant)
- Mermaid diagram (minimum one)
- "Study Drills" section with 5–10 quick questions
- References: "PHAK Ch <#> (heading/subheading/page if available)"

Formatting rules:
- Use H1 title matching the concept
- Use callouts sparingly (e.g., > [!tip], > [!warning]) if your vault style supports it
- Use Obsidian links to related concepts (at least 3 per note)

Also:
- Add 15–30 new oral Q/A items from this chapter into 08-Oral-Exam/Oral-QA.md.
- Update 00-Study-Plan/ACS-Mapping.md: map created notes to likely ACS areas/tasks.

Proceed now and write files into the repo.
In this Obsidian vault repo, create a practical FAR/AIM notes pack for Private Pilot (PPL).

Scope (keep it PPL relevant):
- FAR Part 61: eligibility, medical, currency, endorsements basics (no deep commercial/ATP)
- FAR Part 91: VFR basics, right-of-way, minimum safe altitudes, fuel requirements, required documents, equipment basics
- AIM: focus on VFR communication basics, airport operations, traffic patterns, airspace/pilot responsibilities

Rules:
- Do not fabricate regulation numbers. If you cite a specific FAR, be accurate.
- When unsure, use a "Verify FAR reference" TODO and describe the rule in plain English.
- Create concept notes, not a wall of regulations.

Deliverables:
- 01-Regulations/Regulations-Index.md (if missing)
- Separate notes for each major concept:
  - Required Documents (ARROW)
  - VFR Weather Minimums overview + table by airspace
  - Right-of-Way rules
  - Fuel requirements (day/night VFR)
  - Equipment requirements basics (and how to think about INOP equipment)
  - Currency vs proficiency
  - Logging PIC / endorsements basics (high-level, PPL focused)
- Include at least 2 Mermaid diagrams (e.g., "Decision tree: Is this flight legal?" or "Airspace → minima lookup flow")
- Add 50 oral Q/A items into 08-Oral-Exam/Oral-QA.md for regs.

Update indexes and ACS mapping.

Write all files into the repo now.
Create a concept note in this Obsidian vault repo titled:
"<CONCEPT_NAME>.md"

Primary objective:
Teach the concept using diagrams and step-by-step reasoning.

Must include:
- 3 diagrams:
  1) Mermaid flowchart for cause → effect or decision logic
  2) Mermaid mindmap breaking down subtopics
  3) A compact ASCII sketch if the concept benefits from it (e.g., airflow, stability axes, pressure systems)
- "Misconceptions" section with at least 5 common incorrect beliefs and corrections
- "Oral Exam Drill" section: 15 questions with short model answers
- Link to at least 5 related vault concepts using [[...]]
- References to source docs (PHAK, ACS, FAR/AIM) if applicable

Write file in the correct folder based on vault structure and update the relevant index note.
Open and append to:
08-Oral-Exam/Oral-QA.md

Generate 60 new Private Pilot oral exam questions with answers.
Requirements:
- Mix: 40 knowledge, 15 scenario-based ADM, 5 "trick" questions (with explanation)
- Tag each question with:
  - Topic tag (e.g., #weather #airspace #regs #aero #systems #nav #humanfactors #performance)
  - Suggested ACS area/task (best effort)
- Answers must be brief, correct, and checkride-friendly.
- Add cross-links to existing concept notes in this vault using [[...]].
- If you are unsure on a regulation number, do not cite it; phrase as a concept and add TODO to verify.

Append only; do not delete existing content.
