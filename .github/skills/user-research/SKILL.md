---
name: user-research
description: "Use when: planning user research, generating research hypotheses, creating survey questions, writing user interview questions, validating product assumptions, synthesizing UX insights, analyzing transcripts, processing research inputs (one-pagers, specs, MBR docs, interview transcripts). Produces hypothesis document, survey question list, and interview question list stored in their respective folders. Invoke with /user-research or describe your research context."
argument-hint: "Paste your inputs here: product spec, transcript, one-pager, MBR doc, or describe the problem space"
---

# User Research Skill

A structured research assistant workflow that transforms raw inputs into a validated research plan: hypotheses, survey questions, and interview questions.

## When to Use

- Starting a new research initiative with unclear hypotheses
- Have a spec, brief, MBR doc, or transcript and need a research plan
- Need to validate product assumptions before building
- Want to close a research loop with a mix of quantitative (survey) and qualitative (interview) methods
- Have early/partial hypotheses and need to refine them

## Inputs Accepted

See [inputs guide](./references/inputs-guide.md) for how to process each input type.

| Input Type | Stage | Where to Put It |
|---|---|---|
| Product spec / one-pager | Hypothesis generation | `inputs/` folder |
| MBR / business review doc | Hypothesis generation | `inputs/` folder |
| Prior research / literature | Hypothesis generation | `inputs/` folder |
| Internal researcher transcript | Hypothesis refinement | `inputs/` folder |
| Rough / partial hypothesis list | Hypothesis refinement | `hypothesis/` folder |
| Screener criteria | Survey design | `inputs/` folder |
| Existing survey results | Survey refinement | `survey/` folder |
| User interview transcripts | Interview refinement | `interviews/` folder |

## Outputs

| Output | Location | Template |
|---|---|---|
| Hypothesis document | `hypothesis/hypotheses.md` | [Template](./assets/hypothesis-template.md) |
| Survey questions | `survey/survey-questions.md` | [Template](./assets/survey-template.md) |
| Interview questions | `interviews/interview-questions.md` | [Template](./assets/interview-template.md) |

---

## Procedure

### Stage 1 — Hypothesis Generation

**Goal**: Extract the core unknowns and assumptions from inputs and convert them into testable hypotheses.

1. Read all files in `inputs/`. For each file, identify:
   - The product/feature being researched
   - Claimed user behaviors or pain points
   - Business assumptions being made
   - Gaps or unknowns explicitly called out

2. If a draft exists in `hypothesis/`, read it and treat it as a starting point to refine (not replace).

3. Generate hypotheses using the format in [hypothesis guide](./references/hypothesis-guide.md). Each hypothesis must be:
   - Scoped to one observable behavior or belief
   - Testable (can be confirmed or disproved)
   - Tied to a signal (what evidence would validate it)

4. Group hypotheses by theme (e.g., Discovery, Onboarding, Core Value, Retention).

5. Save output to `hypothesis/hypotheses.md` using [hypothesis template](./assets/hypothesis-template.md).

6. **Pause and ask the user to review** before proceeding to Stage 2. Do not auto-proceed.

---

### Stage 2 — Survey Question Design

**Goal**: Design unmoderated survey questions that quantitatively validate each hypothesis.

1. Read `hypothesis/hypotheses.md`.

2. For each hypothesis, design 1–3 survey questions using the methods in [survey guide](./references/survey-guide.md):
   - Use Likert scale for attitude/belief hypotheses
   - Use multiple-choice for behavioral hypotheses
   - Use open-ended for exploratory unknowns

3. Include:
   - A screener section (2–4 questions to qualify respondents)
   - Core validation questions (one per hypothesis)
   - A closing open-ended question

4. Map each question back to the hypothesis it validates (include hypothesis ID).

5. Save output to `survey/survey-questions.md` using [survey template](./assets/survey-template.md).

6. **Pause and ask the user to review** before proceeding to Stage 3.

---

### Stage 3 — Interview Question Design

**Goal**: Design moderated user interview questions that probe deeper where survey data is insufficient.

1. Read `hypothesis/hypotheses.md` and `survey/survey-questions.md`.

2. Identify which hypotheses need qualitative depth (complex behaviors, emotional responses, context-dependent actions).

3. Design interview questions using the structure in [interview guide](./references/interview-guide.md):
   - Warm-up (2–3 questions: background, context)
   - Core probes (1–2 questions per hypothesis, open-ended)
   - Scenario / task walk-throughs where applicable
   - Closing (what matters most to you, anything we missed)

4. Structure the guide with estimated time per section (total: 45–60 min).

5. Save output to `interviews/interview-questions.md` using [interview template](./assets/interview-template.md).

6. **Present summary** of all three outputs and ask the user to confirm before committing.

---

## Review Gate

Before writing any file, summarize the proposed output and ask:

> "Here's what I'm planning to write to `[file path]`. Shall I proceed?"

Only write files after receiving explicit confirmation or the user says "go ahead / looks good / yes".

## Commit Guidance

Once all three stages are reviewed and approved:
```
git add hypothesis/ survey/ interviews/
git commit -m "research: add hypotheses, survey, and interview questions for [topic]"
```
