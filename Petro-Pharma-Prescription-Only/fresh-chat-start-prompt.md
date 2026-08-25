# Fresh-Chat Start Prompt — Petro-Pharma Prescription-Only

Copy everything in the code block below and paste it into a new chat window that is pointed at the `united snakes of pedomerica` project space. That is all you need to do to begin.

---

```
Use the project-space research standards already in force for this repository and treat them as binding for this entire session.

We are working on the branch/topic: Petro-Pharma-Prescription-Only
Repository: https://github.com/knowurknottty/RAW-research/tree/Petro-Pharma-Prescription-Only

Workflow file: Petro-Pharma-Prescription-Only/prescription_research_workflow.md
Base list file: Petro-Pharma-Prescription-Only/base_prescription_50.csv

The full workflow is defined in the workflow file above. Read it before beginning.
The base list of 50 prescription drugs is in the CSV file above. That is the authoritative source queue.

Research cadence:
- Audit exactly four drugs per block, in rank order, starting with rows 1–4.
- After completing exactly four rows, stop at a clean break and wait for me to type `cont`.
- When I type `cont`, continue with the next four rows from the exact stopping point.
- Do not restart. Do not re-introduce. Do not summarize prior blocks unless precision requires it.
- If you detect session drift (outputs shortening, citations thinning, hedges accumulating beyond what evidence warrants), name it explicitly and stop. Wait for `cont` before resuming.

Per-drug audit steps (summary — full detail in workflow file):
1. Identify the 2–3 most common U.S. prescription formulations for each drug.
2. Pull primary-source inactive ingredient data from FDA DailyMed (dailymed.nlm.nih.gov) or official prescribing information.
3. Flag petrochemical-linked excipients: PEG, propylene glycol, polysorbate 80, sodium lauryl sulfate, parabens, benzyl alcohol, synthetic polymer coatings, HFA propellants, FD&C dyes, and related synthetic compounds.
4. Note active ingredient synthesis pathway where documented in primary sources.
5. Preserve counterevidence — cleaner formulations, reformulations, trace-amount caveats.
6. Classify each drug as exactly one of:
   - Strong direct positive
   - Formulation-dependent positive
   - Unresolved
   - Negative for surfaced formulation only

Output per block:
- An audit table with columns: row #, generic drug, formulations audited, classification, key petrochem-linked ingredients, key counterevidence, note.
- Evidence classification labels on every factual claim ([PRIMARY-SOURCE], [INFERENCE], [UNRESOLVED], etc.).
- A short carry-forward notes section.

Research standard:
- Primary sources first. DailyMed > FDA label database > manufacturer PI sheets.
- Preserve counterevidence. Never suppress a narrowing fact.
- Treat uncertainty as information — label it [UNRESOLVED], not as a defect to paper over.
- Do not universalize from one dosage form, one manufacturer, or one year's formulation to all formulations.
- This is a forensic public record, not advocacy. The standard must survive scrutiny from all directions.

Begin now with Block 01: rows 1–4
(Atorvastatin, Levothyroxine, Metformin, Amlodipine)
```

---

*Saved to branch: Petro-Pharma-Prescription-Only by knowurknot.*
