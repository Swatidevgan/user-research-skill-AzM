# Survey Guide

Reference for designing unmoderated survey questions that quantitatively validate hypotheses.

---

## Survey Structure

A complete survey has three sections:

| Section | Purpose | # of Questions |
|---|---|---|
| Screener | Qualify respondents | 2–4 |
| Core validation | Test each hypothesis | 1–3 per hypothesis |
| Closing | Capture unprompted priorities | 1–2 |

Keep total survey length to **10–15 minutes** (roughly 15–20 questions max).

---

## Question Types by Hypothesis Type

### Attitude / Belief Hypothesis → Likert Scale
Use when the hypothesis is about what users *think* or *feel*.

```
"[Statement reflecting the hypothesis belief]"
○ Strongly Agree  ○ Agree  ○ Neutral  ○ Disagree  ○ Strongly Disagree
```

Example: "I find it easy to understand what this product does in the first 5 minutes."

### Behavioral Hypothesis → Multiple Choice or Frequency
Use when the hypothesis is about what users *do*.

```
"How often do you [behavior]?"
○ Daily  ○ Weekly  ○ Monthly  ○ Rarely  ○ Never
```

Or:
```
"When you [situation], which of the following do you do? (Select all that apply)"
□ Option A  □ Option B  □ Option C  □ Other: ____
```

### Exploratory Unknown → Open-Ended
Use when you need to discover patterns, not validate a known hypothesis.

```
"What is the single biggest challenge you face when [context]?"
[Text box]
```

Limit to 1–2 open-ended questions per survey to preserve completion rate.

---

## Screener Design

The screener ensures you're collecting data from the right users.

Always include:
- **Role / job function** (if user type matters)
- **Product usage frequency** ("How often do you use [product]?")
- **Feature familiarity** (if testing a specific feature)
- **Company size** (if targeting SMB vs. enterprise)

Disqualify respondents who don't match your target before they reach the core survey.

---

## Question Writing Rules

- [ ] One idea per question — never combine two conditions with "and"
- [ ] Avoid leading language ("Don't you think...?", "How great was...?")
- [ ] Use plain language — no jargon unless your target audience is technical
- [ ] For Likert scales, keep the statement positive (negated statements confuse respondents)
- [ ] Every question traces to a hypothesis ID — if it doesn't, cut it

---

## Hypothesis Mapping

Add a mapping table at the top of the survey document:

| Survey Question ID | Hypothesis ID | Type |
|---|---|---|
| Q4 | H1 | Likert |
| Q5 | H2 | Multiple choice |
| Q8 | H3, H4 | Open-ended |

---

## Closing Section

End every survey with:

1. A ranking or forced-choice question about priorities:
   > "Which of the following is most important to you? (Select one)"

2. An open-ended catch-all:
   > "Is there anything else you'd like us to know about your experience with [topic]?"
