# COPD Management Decision Support Tool

Guideline-mapped workflow for COPD evaluation and management based on the 2026 Global Initiative for Chronic Obstructive Lung Disease Clinical Practice Guidelines.

## Overview

This repository contains a browser-based clinical decision support prototype for clinicians managing chronic obstructive pulmonary disease (COPD). The tool is designed to make GOLD 2026 treatment logic easier to apply at the point of care by structuring assessment, surfacing treatment pathways, and generating a copy/paste-ready plan for documentation.

It is intended as a clinician support tool, not as an autonomous medical decision maker.

## Current capabilities

- Separates initial pharmacologic management from follow-up pharmacologic management.
- Assigns GOLD A/B/E grouping from symptom burden and exacerbation history.
- Includes built-in CAT and mMRC calculators.
- Notes that higher CAT scores correlate with worse symptom burden.
- Applies eosinophil-aware inhaled corticosteroid escalation logic.
- Adds dosing and administration guidance when roflumilast, azithromycin, ensifentrine, dupilumab, or mepolizumab are triggered.
- Prompts for smoking cessation treatment options, vaccine recommendations, alpha-1 antitrypsin deficiency screening, and lung cancer screening eligibility.
- Flags advanced-disease considerations such as LTOT, NIV, lung volume reduction referral, and palliative/supportive care review.
- Generates a copy/paste-ready clinical note summarizing the case and plan.

## Quick start

This is a static web app. No build step or server framework is required.

1. Clone the repository.
2. Open `index.html` in a modern browser.
3. Enter the patient-specific data.
4. Review the generated treatment plan, prevention prompts, medication details, and note output.

If you prefer to serve it locally:

```bash
python3 -m http.server 8765
```

Then open `http://127.0.0.1:8765/`.

## Repository contents

- `index.html`: application UI
- `app.js`: decision logic and note generation
- `styles.css`: layout and visual styling

## Evidence approach

The current implementation is mapped primarily to:

- GOLD 2026 Report v1.3 (December 8, 2025)
- Current Centers for Disease Control and Prevention guidance for adult vaccination
- American Cancer Society lung cancer screening guidance
- Official prescribing information for medication-specific dosing and administration details

Reference page:

- [GOLD 2026 report and pocket guide](https://goldcopd.org/2026-gold-report-and-pocket-guide/)

## Important repository note

The local GOLD PDF and teaching slide deck used during development are intentionally not committed here. They are copyrighted source materials and should be obtained directly from the official GOLD distribution channels.

## Clinical disclaimer

This project is for clinician support only. It does not replace clinical judgment, full patient assessment, contraindication review, local formulary restrictions, or institutional/national policy.

## Status

This is an actively evolving prototype. The current sharable branch is:

- `codex/copd-management-tool`

GitHub repository:

- [abhimanyuchandel/COPD-DECISION-SUPPORT](https://github.com/abhimanyuchandel/COPD-DECISION-SUPPORT)

## License

MIT. See the `LICENSE` file.
