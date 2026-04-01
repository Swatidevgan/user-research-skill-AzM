# User Research Skill (GH Copilot)
Initial user research skill templates


This repo defines a repeatable User Research Skill for GitHub Copilot in VS Code.

The skill does three things:
1. Generate research hypotheses from inputs
2. Design unmoderated survey questions to validate hypotheses
3. Design moderated user interview questions to close gaps

Copilot acts as a research assistant. Outputs are structured, testable, and review-ready before you commit.

---

## Getting Started

### 1. Clone and open in VS Code
```bash
git clone <repo-url>
cd user-research-skill
code .
```

### 2. Add your inputs

Drop any of the following into the `inputs/` folder before starting:
- Product spec or one-pager
- MBR / business review doc
- Prior research docs
- Internal researcher conversation transcript
- Draft hypothesis list (drop in `hypothesis/` instead)

### 3. Invoke the skill

In VS Code Copilot Chat, type:
```
/user-research
```
Or describe your context in chat — Copilot will recognize the research domain and load the skill automatically.

Paste your inputs directly into chat, or reference files already in `inputs/`.

### 4. Review before commit

The skill pauses after each stage for your review. Once all three outputs look good:
```bash
git add hypothesis/ survey/ interviews/
git commit -m "research: add hypotheses, survey, and interview questions for [topic]"
```

---

## Folder Structure

```
inputs/          ← Drop your raw inputs here (specs, docs, transcripts)
hypothesis/      ← Generated: hypotheses.md
survey/          ← Generated: survey-questions.md
interviews/      ← Generated: interview-questions.md

.github/
  skills/
    user-research/
      SKILL.md                        ← Skill definition (entry point)
      references/
        inputs-guide.md               ← How to process each input type
        hypothesis-guide.md           ← Hypothesis format and quality rules
        survey-guide.md               ← Survey question design guide
        interview-guide.md            ← Interview question design guide
      assets/
        hypothesis-template.md        ← Output template
        survey-template.md            ← Output template
        interview-template.md         ← Output template
```

---

## Skill Stages

| Stage | Input | Output | Location |
|---|---|---|---|
| 1. Hypothesis | Files in `inputs/` | `hypotheses.md` | `hypothesis/` |
| 2. Survey | `hypothesis/hypotheses.md` | `survey-questions.md` | `survey/` |
| 3. Interview | `hypothesis/hypotheses.md` + `survey/` | `interview-questions.md` | `interviews/` |

Each stage pauses for review before proceeding to the next.