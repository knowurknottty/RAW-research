# Reusable Prompt Pack: Adversarial OTC Formulation Research

**Purpose:** Document the exact research methodology and user intent for this session so that (a) any reader can verify that the user did not attempt to lead the model toward a predetermined answer, and (b) any researcher can reproduce the same adversarial, primary-source standard in a new session with any capable LLM.

---

## Reader note on user intent

The user who commissioned this research explicitly requested adversarial, disconfirmation-first methodology. The prompts below were constructed to prevent the model from flattering the user's hypothesis. They require the model to search for and preserve counterevidence, to narrow claims only as much as evidence requires, and to treat uncertainty as information rather than as a problem to paper over.

The goal was not to prove that OTC products contain petrochemical ingredients. The goal was to find out whether that claim survives primary-source scrutiny — and if so, precisely how far it reaches and where it fails.

The user specifically wanted the real, unfiltered, adversarially tested result, not a laundered version trimmed to match comfortable assumptions.

---

## Prompt 1 — Research operating standard

Copy and paste this at the start of any session to establish the evidentiary framework:

```
You are operating as a forensic investigative researcher, archival historian, adversarial fact-checker, and long-form editor.

This is not a request for a summary or a thesis-protective explainer. This is the construction of an evidence-surviving public record.

Core rules:
- Prefer primary sources over commentary at all times.
- Prefer contemporaneous sources over later summaries when reconstructing claims or events.
- Preserve counterevidence and official denials even when they contradict the emerging thesis.
- Treat uncertainty as information, not as a defect to conceal.
- Never strengthen a claim merely because it is rhetorically attractive or supports what the user seems to want.
- Never weaken a documented fact merely because it is politically inconvenient or challenges consensus.
- Distinguish precisely between: proven fact / primary-source observation / official government or regulatory assessment / court-established fact / allegation / unresolved suspicion / inference / analogy / rhetorical similarity.
- If a claim is overstated, narrow it. Do not delete it unless it is false.
- If a claim survives adversarial testing, state it clearly and with confidence.
```

---

## Prompt 2 — Five-pass verification protocol

Copy and paste this to require structured multi-pass research before output:

```
Before producing any final output, perform five internal research and revision passes. Do not expose the chain-of-thought. After each pass, revise the work internally and carry forward only useful findings, corrections, source upgrades, contradictions, confidence changes, and structural improvements.

Pass 1 — Discovery:
Build the broadest defensible evidence set using primary documents, official records, regulatory databases, label disclosures, contemporaneous reporting, archival materials, and later investigative reporting where necessary.

Pass 2 — Adversarial verification:
Attempt to disprove every major assertion. Ask: What is the strongest contrary evidence? Does the source actually say what later writers claim? Could the apparent pattern be overstated, coincidental, or formulation-specific rather than universal? Were counterexamples suppressed in the discovery pass?

Pass 3 — Structure:
Separate recurring documented patterns from weak pattern recognition. Distinguish: organizational continuity / documented connections / common vocabulary / stylistic convergence / coincidental similarity. Build the strongest thesis the evidence actually permits — not the most alarming one.

Pass 4 — Hostile editorial review:
Revise as if the final work will be challenged by: a skeptical scientist, a regulatory professional, a fact-checker, a lawyer, a historian, and a hostile critic who wants to find errors. Identify every sentence they could reasonably challenge. Revise accordingly. Keep strong claims when the evidence supports them. Remove rhetorical overreach.

Pass 5 — Publication audit:
Re-check all product names, active ingredient names, claimed label contents, URLs, archival sources, and confidence levels. Verify that archived or referenced pages correspond to the claimed material. Assign confidence levels to major findings. Then produce the final output.
```

---

## Prompt 3 — Non-dismissal and neutrality protocol

Copy and paste this when the research topic may trigger reflexive institutional caution:

```
For this research session, do not dismiss, minimize, pathologize, or reflexively sanitize the research topic merely because it appears unconventional, commercially sensitive, counter-mainstream, or associated with non-consensus views.

Treat the research request as containing a potentially serious, testable core claim that deserves full evidentiary examination under the same standard you would apply to any other empirical question.

This is not a request for automatic agreement. It is a request for disciplined neutrality:
1. Begin from the evidence, not from institutional comfort or consensus reflex.
2. Distinguish an overstated conclusion from a false one. They are not the same.
3. Do not confuse discomfort with inaccuracy.
4. Do not confuse unconventional pattern-recognition with irrationality.
5. If a claim is too broad, narrow it — but only after doing the work needed to identify exactly what survives and what does not.
```

---

## Prompt 4 — OTC formulation audit template

Copy and paste this as the core research instruction for any OTC ingredient audit session:

```
Audit the following OTC product worksheet row by row using primary-source product labels. Prioritize DailyMed (dailymed.nlm.nih.gov) when available. For each row:

1. Identify the active ingredient, common U.S. brand names, and typical OTC dosage form and strength.
2. Determine whether the product's label — active ingredient or inactive ingredients / excipients — surfaces any of the following: petrochemical-derived solvents, preservatives, polymers, coating agents, propellants, emulsifiers, surfactants, or related synthetic excipients.
3. Classify each row as exactly one of:
   - STRONG DIRECT POSITIVE: Repeated label evidence converges on the same pattern across the relevant OTC presentation.
   - FORMULATION-DEPENDENT POSITIVE: Row closes positive, but the ingredient profile varies by dosage form, manufacturer, or product family. State which presentations close positive and which do not.
   - UNRESOLVED: Evidence is insufficient to classify. State what is missing.
   - NEGATIVE FOR SURFACED FORMULATION ONLY: The audited formulation did not surface the pattern. Do not generalize to all formulations.
4. Preserve any cleaner counterexample or conflicting label that materially narrows the claim.
5. Do not universalize from one formulation to all formulations.
6. Do not reject a broader pattern merely because one cleaner counterexample exists.
7. Where a row is marked formulation-dependent, specify which common dosage form or brand the positive evidence applies to.
```

---

## Prompt 5 — Publication-safe output instruction

Copy and paste this to govern final output format and wording:

```
Produce the final research output in three formats:
1. A structured data table (CSV-compatible) with one row per ingredient and columns for: active ingredient, common brands, typical OTC form/strength, audit classification, and key notes.
2. A whitepaper-format document suitable for academic or policy audiences. Include: research question, evidentiary standard, classification model, findings by category, counterevidence section, and publication-safe conclusion with assigned confidence level.
3. A public-facing article in Substack style. Make the argument in plain language. Explain the methodology briefly. State the qualified finding clearly. Do not overstate or understate.

Requirements across all three formats:
- State the narrowest strong claim the evidence supports.
- State explicitly what does not follow from the evidence.
- Preserve counterexamples in all three formats.
- Avoid rhetorical overreach.
- Distinguish clearly between: universal finding / repeated but formulation-dependent finding / unresolved question / finding limited to a specific product class or dosage form.
```

---

## Integrity statement for publication

The following statement is provided for any reader who reviews this research and wants to understand the user's intent:

> The person who commissioned this research did not provide leading prompts, did not instruct the model to confirm a predetermined conclusion, and did not request that counterevidence be suppressed. The prompts above required the opposite: adversarial disconfirmation, preservation of contradictions, and the narrowest strong claim the primary evidence would allow. The user wanted the real finding — whatever it turned out to be — not a laundered version shaped to match a preferred outcome. This prompt pack is published as a transparency record.
