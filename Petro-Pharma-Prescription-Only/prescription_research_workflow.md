# Petro-Pharma Prescription-Only — Research Workflow

**Repository:** knowurknottty/RAW-research  
**Branch:** Petro-Pharma-Prescription-Only  
**Operator:** knowurknot  
**Standard:** Forensic investigative / adversarial fact-check / publication-ready  
**Continuity signal:** User types `cont` to advance. No re-introduction. No restart.

---

## Purpose

This workflow governs the systematic audit of petrochemical-linked ingredients in the 50 most-prescribed U.S. prescription drugs (2024 data). The base source list is `base_prescription_50.csv` in this branch. Research is conducted four drugs at a time, with a mandatory stop-and-wait after each block. Results accumulate into `prescription_research_table.csv`, and final deliverables are `prescription_research_whitepaper.md`, `prescription_research_substack_article.md`, and `prescription_research_prompt_pack.md`.

The goal is a fully transparent, adversarially verified, primary-source-grounded public record — not advocacy, not debunking, and not endorsement.

---

## Base Source List

File: `base_prescription_50.csv`  
Columns: rank, generic_drug, major_us_brands, class, principal_uses, rx_2024, patients_2024, delta_vs_2023  
Rows: 50 (Atorvastatin through Spironolactone)

---

## Four-at-a-Time Cadence

1. Audit exactly four drugs per block, in rank order.
2. After completing four rows, stop at a clean break point.
3. Await the user typing `cont` before continuing to the next four.
4. Do NOT restart. Do NOT summarize prior blocks unless precision requires it.
5. If SESSION DRIFT is detected (outputs shortening, citations thinning, hedges accumulating beyond what evidence warrants), name it explicitly, identify the last fully-verified claim, stop, and wait for `cont`.

Blocks:
- Block 01: rows 1–4   (Atorvastatin, Levothyroxine, Metformin, Amlodipine)
- Block 02: rows 5–8   (Lisinopril, Albuterol, Losartan, Metoprolol)
- Block 03: rows 9–12  (Rosuvastatin, Omeprazole, Gabapentin, Sertraline)
- Block 04: rows 13–16 (Escitalopram, Semaglutide, Mixed amphetamine salts, Pantoprazole)
- Block 05: rows 17–20 (Bupropion, Hydrochlorothiazide, Fluoxetine, Trazodone)
- Block 06: rows 21–24 (Montelukast, Amoxicillin, Fluticasone, Tamsulosin)
- Block 07: rows 25–28 (Apixaban, Simvastatin, Insulin glargine, Empagliflozin)
- Block 08: rows 29–32 (Furosemide, Meloxicam, Hydrocodone/acetaminophen, Tirzepatide)
- Block 09: rows 33–36 (Methylphenidate, Duloxetine, Prednisone, Carvedilol)
- Block 10: rows 37–40 (Famotidine, Ibuprofen, Buspirone, Venlafaxine)
- Block 11: rows 41–44 (Tramadol, Potassium chloride, Hydroxyzine, Allopurinol)
- Block 12: rows 45–48 (Clopidogrel, Ergocalciferol, Cetirizine, Ondansetron)
- Block 13: rows 49–50 (Cyclobenzaprine, Spironolactone) — final block

---

## Per-Drug Audit Steps

For each drug in the block:

**Step 1 — Identify representative formulations**  
Identify the 2–3 most common prescription formulations for ordinary U.S. clinical use (e.g., immediate-release tablet, extended-release capsule, injectable). Do not audit every formulation — audit the most prescribed ones. State which formulations you are auditing.

**Step 2 — Pull primary-source label data**  
Primary source: FDA DailyMed (dailymed.nlm.nih.gov). Secondary fallback: FDA drug label database, manufacturer prescribing information PDFs. Do not use consumer summaries, Wikipedia, or advocacy sites as evidence.

**Step 3 — Audit inactive ingredients for petrochemical-linked substances**  
Flag any of the following categories if present:
- Petroleum-derived solvents (e.g., polyethylene glycol, propylene glycol, mineral oil)
- Synthetic polymers used as coatings or binders (e.g., polyvinyl alcohol, hypromellose, Eudragit/methacrylic acid copolymers, polyvinylpyrrolidone/povidone, polysorbate 80)
- Petroleum-derived preservatives (e.g., benzyl alcohol, methylparaben, propylparaben)
- Synthetic surfactants (e.g., sodium lauryl sulfate)
- Propellants (e.g., HFA-134a, HFA-227ea — hydrofluoroalkane propellants used in inhalers; note these are synthetic fluorinated compounds, not petroleum-derived in the crude-oil sense, and must be labeled accordingly)
- Petroleum-derived plasticizers (e.g., triethyl citrate when used as a plasticizer; dibutyl sebacate)
- Synthetic colorants with petroleum precursors (e.g., FD&C dyes)

**Step 4 — Audit active ingredient synthesis pathway (where documented)**  
Note where the active pharmaceutical ingredient itself is synthesized via petrochemical feedstocks (e.g., benzene-derived intermediates, toluene-derived intermediates). Label this as [INFERENCE] or [SCHOLARLY] unless a primary source documents the feedstock chain directly.

**Step 5 — Preserve counterevidence**  
For each drug, identify and state the strongest counterevidence or narrowing fact:
- Are there common formulations of the same drug that do NOT contain the flagged ingredients?
- Are there generic alternatives with cleaner excipient profiles?
- Does the flagged ingredient appear in a trace amount unlikely to be systemically relevant?
- Has the manufacturer reformulated to remove the ingredient?
Counterevidence must not be suppressed.

**Step 6 — Assign classification**  
Choose exactly one:
- **Strong direct positive** — petrochemical-linked synthetic excipients or active synthesis chain documented from a primary source across the dominant formulations.
- **Formulation-dependent positive** — petrochemical-linked ingredients present in some but not all common formulations; cleaner alternatives exist.
- **Unresolved** — label data is incomplete, conflicting, or the petrochemical linkage is indirect and requires further evidence.
- **Negative for surfaced formulation only** — audited formulations do not surface petrochemical-linked ingredients; this classification applies only to the specific formulations reviewed, not all formulations ever manufactured.

---

## Output Format Per Block

### Audit Table

| # | Generic drug | Formulations audited | Classification | Key petrochem-linked ingredients | Key counterevidence | Note |
|---|---|---|---|---|---|---|

All entries must carry evidence classification labels from the project standard:
[PRIMARY-SOURCE], [INVESTIGATIVE-REPORTING], [INFERENCE], [UNRESOLVED], etc.

### Carry-Forward Notes
After the table: a short bulleted list of items the later whitepaper and Substack export must preserve — ambiguities, unresolved threads, strongest counterarguments, formulations not yet audited.

---

## Final Deliverables (assembled after Block 13 is complete)

| File | Purpose |
|---|---|
| `prescription_research_table.csv` | Full 50-row audit table, all columns |
| `prescription_research_whitepaper.md` | Policy/academic long-form write-up |
| `prescription_research_substack_article.md` | Public-facing article, publication-safe |
| `prescription_research_prompt_pack.md` | Full methodology and prompt record |

---

## Evidence Classification Reference

| Label | Meaning |
|---|---|
| [COURT-ESTABLISHED] | Court record, indictment, plea, or judicial finding |
| [DECLASSIFIED-GOV] | Declassified U.S. government document |
| [OFFICIAL-ASSESSMENT] | Official U.S. government agency assessment |
| [CONGRESSIONAL-RECORD] | GAO, CRS, congressional hearing or record |
| [PRIMARY-SOURCE] | Original document, transcript, label, or database entry |
| [ARCHIVED-PRIMARY] | Wayback Machine / archived copy of deleted primary source |
| [CONTEMPORANEOUS-REPORTING] | Journalism published within 30 days of the event |
| [INVESTIGATIVE-REPORTING] | Later investigative journalism with named sources |
| [SCHOLARLY] | Peer-reviewed or archival historical scholarship |
| [ALLEGATION] | Stated by interested party; not independently verified |
| [UNRESOLVED] | Conflicting evidence; no resolution available |
| [INFERENCE] | Logical derivation from established facts; not direct evidence |
| [ANALOGY] | Structural/rhetorical similarity; does not establish causation |
| [ADVOCACY-SOURCE] | Explicitly identified; used only when necessary |

---

*This workflow was created by knowurknot. It is binding across all sessions working on this branch.*
