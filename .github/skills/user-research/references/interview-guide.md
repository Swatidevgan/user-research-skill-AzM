# Interview Guide

Reference for designing moderated user interview question guides that close gaps the survey cannot address.

---

## Interview Structure

A standard 45–60 minute interview follows this arc:

| Section | Duration | Purpose |
|---|---|---|
| Warm-up | 5 min | Build rapport, establish context |
| Background | 5–10 min | Understand the user's role and workflow |
| Core probes | 20–30 min | Dig into hypothesis-specific behaviors |
| Scenario / task | 5–10 min | Observe behavior in a realistic context (optional) |
| Closing | 5 min | Capture unprompted priorities and wrap up |

---

## Question Types

### Open-Ended (default)
Use for most questions. Never asks for yes/no.

> "Tell me about the last time you [behavior]."  
> "Walk me through how you currently [task]."  
> "What does [X] mean to you?"

### Probing Follow-ups
Use immediately after an answer to go deeper. Never interrupt — probe after they finish.

> "Can you tell me more about that?"  
> "What happened next?"  
> "Why did you do it that way?"  
> "How did that make you feel?"  
> "What would have made that easier?"

### Scenario / Hypothetical
Use carefully and only to explore mental models, not validate behavior.

> "Imagine you had to [situation]. How would you approach that?"  
> "If [feature] existed, how would you use it in a typical week?"

Avoid asking "would you use this?" — users overestimate their future adoption.

### Closing Questions
Always end with:

> "Is there anything about [topic] that we haven't covered that feels important?"  
> "What's the single most important thing that would improve your experience with [context]?"

---

## Mapping Interviews to Hypotheses

For each hypothesis you want to probe:

1. Write 1 **scene-setting question** (what they do today, without mentioning your solution)
2. Write 1–2 **probing questions** (dig into the behavior or belief)
3. Prepare 2–3 **follow-up probes** in case answers are shallow

Example for **H2 — Onboarding — Time to first value**:

> Scene: "Tell me about the first time you used [product]. What were you trying to do?"  
> Probe: "When did you feel like you 'got it'? What made that click?"  
> Follow-up: "What would have helped earlier in that experience?"

---

## Interviewer Rules

- Do not lead with solutions: never say "we're thinking of adding X, what do you think?"
- Do not validate out loud: avoid saying "great" or "interesting" in a way that signals right/wrong answers
- Let silence breathe: wait 3–5 seconds after an answer before probing
- Take verbatim notes on emotional language — exact quotes matter more than paraphrasing
- Flag moments where behavior contradicts stated belief (common: "I never do X" then describes doing X)

---

## Interview vs. Survey: When to Use Each

| Use Interview When | Use Survey When |
|---|---|
| The hypothesis involves context or emotion | The hypothesis is binary (yes/no, often/never) |
| You need to understand *why*, not just *what* | You need statistical confidence across a large sample |
| The behavior is complex or multi-step | You need to prioritize across many users quickly |
| Results from the survey were ambiguous | You already know the answer choices |

---

## Recruiting Notes

- Target 5–8 participants per user segment for qualitative saturation
- Mix of users (new, established, power) unless segment is already scoped
- Avoid recruiting only advocates — include users who churned or disengaged
