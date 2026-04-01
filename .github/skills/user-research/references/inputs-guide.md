# Inputs Guide

Reference for understanding what input types exist, when they're available, and how to extract signals from each.

---

## Input Types

### 1. Product Spec / One-Pager
**What it contains**: Feature description, problem statement, target user, proposed solution, success metrics.  
**Extract**: User assumptions ("users want X"), behavioral claims ("users currently do Y"), business bets ("if we build Z, users will adopt").  
**Treat with skepticism**: Specs often assert user behavior without evidence — these assertions become hypotheses.

### 2. MBR / Business Review Doc
**What it contains**: Business goals, KPIs, pain points from sales/support data, market context.  
**Extract**: Which user segments are struggling, where drop-offs occur, what retention/adoption data suggests.  
**Use for**: Grounding hypotheses in real business pain, not just product assumptions.

### 3. Prior Research / Literature
**What it contains**: Past usability studies, academic papers, competitive analysis, industry benchmarks.  
**Extract**: Validated findings that can be treated as known (reduce hypothesis load), and gaps that still need validation.  
**Prioritize**: Hypotheses where no prior data exists.

### 4. Internal Researcher Transcript
**What it contains**: Back-and-forth notes or a conversation log between you and a research partner or PM.  
**Extract**: Open questions, disagreements on user behavior, things flagged as "we don't actually know this."  
**Treat as**: Raw signal — not validated, but high-quality starting points.

### 5. Rough / Partial Hypothesis List
**What it contains**: An early draft of hypotheses, possibly unstructured.  
**Action**: Load into Stage 1 as a starting point. Reformat to standard structure, fill in gaps, add missing confidence signals.  
**Do not**: Replace it wholesale — refine it.

### 6. Screener Criteria
**What it contains**: Target respondent profile (role, company size, product usage frequency, etc.)  
**Use in**: Stage 2 (Survey) — generates the screener section of the survey.

### 7. Existing Survey Results
**What it contains**: Prior survey responses (quantitative data).  
**Extract**: What was already validated, what remained ambiguous (high variance, unexpected distributions).  
**Use for**: Skipping already-validated hypotheses; adding new ones surfaced by unexpected results.

### 8. User Interview Transcripts
**What it contains**: Verbatim or summarized recordings from moderated sessions.  
**Extract**: Recurring themes, emotional language, workarounds, unmet needs.  
**Use for**: Refining hypotheses with qualitative evidence; updating survey and interview guides for future rounds.

---

## Processing Order

When multiple inputs exist, process in this order:

1. MBR / business doc — establishes what matters to the business
2. Spec / one-pager — establishes what is being built
3. Prior research — eliminates hypotheses already answered
4. Internal transcripts — surfaces open questions and disagreements
5. Draft hypothesis list — establishes starting point for refinement
6. Screener criteria — scopes the research audience

---

## Missing Inputs

If key inputs are absent, note the gap explicitly in the hypothesis document:

> "No prior research available. All hypotheses in the Discovery theme are unvalidated."

Do not fabricate inputs. Ask the user to provide them or flag the dependency.
