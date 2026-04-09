# COPD Management Decision Support Tool

This project is a local, browser-based clinical support tool for structuring COPD management decisions using GOLD 2026 logic.

## What it does

- Assigns GOLD category (A/B/E) from symptom burden and exacerbation history.
- Includes built-in CAT (8-item) and mMRC calculators that auto-fill symptom scores.
- Explicitly separates initial pharmacologic management from follow-up pharmacologic management.
- Applies eosinophil-aware ICS escalation logic and adds dosing guidance for roflumilast, azithromycin, ensifentrine, dupilumab, and mepolizumab when those options are triggered.
- Adds preventive care and screening prompts, including alpha-1 antitrypsin deficiency screening, lung cancer screening eligibility, pneumococcal, RSV, and zoster vaccination guidance.
- Adds smoking-cessation treatment options with dosing and key contraindication reminders for current smokers.
- Surfaces safety checks (spirometry confirmation, asthma coexistence, ICS de-escalation risk, missing screening inputs).
- Generates a copy/paste-ready clinical note summarizing the case and plan.

## How to run

1. Open `/Users/abhichandel/Documents/Research/COPD decision support tool/index.html` in any modern browser.
2. Enter patient data.
3. Click `Generate Management Recommendation`.

No server setup is required.

## Evidence references used in logic

- GOLD 2026 Report v1.3 (December 8, 2025):
  - Report highlights (criteria update and one-moderate-exacerbation threshold)
  - Chapter 3 initial and follow-up pharmacologic algorithm text (Group A/B/E, Figure 3.8 and Figure 3.9 explanatory text)

Reference page:
https://goldcopd.org/2026-gold-report-and-pocket-guide/

## Repository note

The local GOLD PDF and teaching slide deck are not committed to the sharable repository. They are copyrighted reference materials and should be obtained directly from the official GOLD sources.

## Important note

This is a decision-support prototype for clinicians. It is not a substitute for full clinical assessment, local policies, or specialist judgment.
