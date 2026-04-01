# Hypothesis Guide

Reference for generating well-formed, testable research hypotheses.

---

## Hypothesis Format

Use this structure for every hypothesis:

```
**H[N] — [Theme] — [Short label]**

We believe that [USER SEGMENT] [DOES / THINKS / FEELS / STRUGGLES WITH] [BEHAVIOR OR BELIEF]
because [ASSUMED REASON].

We will know this is true when [MEASURABLE SIGNAL OR OBSERVABLE OUTCOME].

Confidence: Low / Medium / High
Priority: P1 / P2 / P3
```

**Fields explained:**
- **User segment**: Be specific (e.g., "first-time users", "enterprise admins", "power users with >50 projects")
- **Behavior/belief**: Observable action, mental model, or attitude — not a design solution
- **Assumed reason**: Your current best guess at the why — this is what gets tested
- **Signal**: What survey response, interview quote, or behavioral metric would confirm or deny this
- **Confidence**: How certain you are this is true *before* research
- **Priority**: How critical this is to validate before shipping

---

## Themes

Group hypotheses under themes to organize the research. Common themes:

| Theme | Focus |
|---|---|
| Discovery | How users find or first encounter the product/feature |
| Onboarding | How users understand and adopt the product for the first time |
| Core Value | Whether the core use case delivers on its promise |
| Collaboration | How users work with others in/around the product |
| Retention | Why users return (or don't) |
| Mental Models | How users think about the problem space |
| Pain Points | Where users currently struggle |

Adapt themes to the specific product or feature being researched.

---

## Generating Hypotheses from Inputs

For each input, ask:

1. **What is being assumed but not proven?** → Becomes a hypothesis
2. **What user behavior is being relied upon?** → Becomes a behavioral hypothesis
3. **What would make this whole plan fail?** → Becomes a high-priority P1 hypothesis
4. **What "we think users want" statements exist?** → Each one is a hypothesis

---

## Quality Checks

A well-formed hypothesis must:

- [ ] Contain exactly one atomic claim (not two claims in one sentence)
- [ ] Be falsifiable — there is a way to disprove it
- [ ] Have a concrete signal (not "we'll know when users are happy")
- [ ] Not embed a solution ("users will love the new button" is not a hypothesis)
- [ ] Not be a certainty ("users need to log in" is a fact, not a hypothesis)

---

## Prioritization

Set priority based on two axes:

| | High Impact on Success | Low Impact on Success |
|---|---|---|
| **Low Confidence** | P1 — Must validate | P2 — Should validate |
| **High Confidence** | P2 — Validate if resources allow | P3 — Skip or monitor |

Aim for 5–10 total hypotheses per research round. More than 10 suggests scope is too broad.
