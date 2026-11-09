# Governing-False-Accusations-and-Abstention-in-AI-Text-Detection

# Submission Package — Governing False Accusations and Abstention in AI Text Detection

## Contents
- `Final_Research_Report.docx` — research report based on the executed `results-6.zip` outputs.
- `code/False_Accusation_Pipeline_TOEFL_Final.ipynb` — revised notebook with TOEFL-only RQ3 scope.
- `code/False_Accusation_Pipeline_TOEFL_Final.py` — Python source export.
- `results/tables/` — CSV result tables.
- `results/figures/` — PDF figures.
- `results/run_manifest.json` — dataset counts, split sizes, scope and limitations.

## Important reproducibility note
The report metrics are taken from the previously executed `results-6.zip`. The notebook has since been edited to make RQ3 explicitly TOEFL-only and to correct output labels. That revised notebook has not yet been executed end-to-end after the scope edit. Do not claim a fresh successful run of the revised notebook until it has been executed and its new ZIP audited.

## Research scope
- RQ3 is a descriptive audit of 91 human TOEFL essays only; no Hewlett/ASAP comparison is claimed.
- The RQ1 script-dominance proxy has only one observed category, so it does not support a between-language comparison.
- RAID metrics are exploratory because the sampled records came from its training split.
- The held-out Reddit model was fitted separately without the sigmoid calibration used by the primary HC3 model; interpret it as a domain-shift diagnostic.

## Key results
- HC3 grouped test accuracy: 98.19%; balanced accuracy: 98.47%; human FPR: 2.29%.
- RQ3 TOEFL audit: 52/91 false accusations (57.14%).
- RQ4: 267 to 125 false accusations (53.18% reduction) at 3.10% abstention.
- RAID train-split exploratory sample: accuracy 65.17%; human FPR 40.13%.

## Reproduction
Run the notebook top-to-bottom in Kaggle or Jupyter with internet enabled. If the optional RAID package is not installed, that section may be skipped. Check all CSVs and the run manifest before submission.
