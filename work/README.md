# work/ — your space

Everything you build lives here: lane experiments, notebooks, figures, and your capstone
report. The rest of the repo is the shared reference; this folder is yours.

## Rules of the road

1. **Copy, don't edit.** Need to change the pipeline? Copy the script here
   (e.g. `work/scripts/03_train_model_v2.py`) or adjust the feature lists in
   `scripts/ml_utils.py`. The reference pipeline in `scripts/` stays pristine — it's the
   baseline you compare against, and reviewers expect to find it unchanged.
2. **No datasets in git.** CSVs inside `work/` are gitignored, and CI fails if any dataset
   CSV is committed anywhere in the repo. Small summary tables belong in your report as
   markdown, not as data files. Metrics JSONs are the opposite: keep files like
   `work/outputs/*.json` **committed** — they are the receipts your report's numbers trace
   back to. Don't add ignore rules that hide them.
3. **Stay reproducible.** Fix your random seeds and note them in your report. Someone with a
   fresh clone should be able to re-run your work from your instructions alone.
4. **Public-safety language.** Everything here may end up public with your submission:
   observed / measured / directional / decision-support — no client-identifying details,
   no causal claims without a design (see `DATA_USE.md`).

## Suggested layout

```text
work/
  notebooks/            your experiment notebooks
  scripts/              copied + modified pipeline pieces
  figures/              charts for your report
  capstone_report.md    your capstone write-up (start from the template)
```

## Capstone

Copy `capstone_report_template.md` to `capstone_report.md` and fill it in as you go — it
mirrors the eight axes your work is graded on, so writing it early keeps you honest.

## Your assignment index

Your skeleton notebooks are already in `notebooks/` — one per assignment, pre-named.
Tick them off as you go; this table is the map of your work (each badge opens the notebook
in Colab, straight from your repo):

| Notebook | Assignment | Open | Status |
|---|---|---|---|
| `notebooks/w01_research_question.ipynb` | ML-02 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Shouban7866/flyrank-ml-internship/blob/main/work/notebooks/w01_research_question.ipynb?flush_cache=true) | ☐ |
| `notebooks/w02_ml_task_framing.ipynb` | ML-03 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Shouban7866/flyrank-ml-internship/blob/main/work/notebooks/w02_ml_task_framing.ipynb?flush_cache=true) | ☐ |
| `notebooks/w03_data_contract.ipynb` | ML-04 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Shouban7866/flyrank-ml-internship/blob/main/work/notebooks/w03_data_contract.ipynb?flush_cache=true) | ☐ |
| `notebooks/w03_feature_leakage_check.ipynb` | ML-05 — optional stretch (card retired 2026-07-13; its core lives in ML-04 now) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Shouban7866/flyrank-ml-internship/blob/main/work/notebooks/w03_feature_leakage_check.ipynb?flush_cache=true) | optional |
| `notebooks/w04_signal_audit.ipynb` | ML-06 — optional stretch (card retired 2026-07-13; its core lives in ML-07 now) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Shouban7866/flyrank-ml-internship/blob/main/work/notebooks/w04_signal_audit.ipynb?flush_cache=true) | optional |
| `notebooks/w04_baseline_score.ipynb` | ML-07 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Shouban7866/flyrank-ml-internship/blob/main/work/notebooks/w04_baseline_score.ipynb?flush_cache=true) | ☐ |
| `notebooks/w05_model.ipynb` | ML-08 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Shouban7866/flyrank-ml-internship/blob/main/work/notebooks/w05_model.ipynb?flush_cache=true) | ☐ |
| `notebooks/w06_validation_audit.ipynb` | ML-09 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Shouban7866/flyrank-ml-internship/blob/main/work/notebooks/w06_validation_audit.ipynb?flush_cache=true) | ☐ |
| `notebooks/w07_action_playbook.ipynb` | ML-10 | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Shouban7866/flyrank-ml-internship/blob/main/work/notebooks/w07_action_playbook.ipynb?flush_cache=true) | ☐ |
| `notebooks/capstone.ipynb` | ML-11 (the paper mirrors it) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Shouban7866/flyrank-ml-internship/blob/main/work/notebooks/capstone.ipynb?flush_cache=true) | ☐ |
| closing section of `notebooks/capstone.ipynb` | ML-12 — 5-min demo outline + social-post cut + employer-facing summary | (same notebook, last markdown cells) | ☐ |

When your paper is deployed, put its exact URL in `../submission/paper_url.txt` (one line).
ML-12 lives in your capstone notebook's closing markdown cells — it's the smallest card and
the easiest to forget, which is exactly why it has a row here.

---

# My Internship Work

## Completed Assignments

I completed the FlyRank Machine Learning Internship workflow from research question definition to the final capstone project.

| Assignment | Notebook | Status |
|------------|----------|--------|
| ML-02 Research Question | w01_research_question.ipynb | ✅ Completed |
| ML-03 ML Task Framing | w02_ml_task_framing.ipynb | ✅ Completed |
| ML-04 Data Contract | w03_data_contract.ipynb | ✅ Completed |
| ML-05 Feature Leakage Check (Optional) | w03_feature_leakage_check.ipynb | ✅ Completed |
| ML-06 Signal Audit (Optional) | w04_signal_audit.ipynb | ✅ Completed |
| ML-07 Baseline Score | w04_baseline_score.ipynb | ✅ Completed |
| ML-08 Model Development | w05_model.ipynb | ✅ Completed |
| ML-09 Validation Audit | w06_validation_audit.ipynb | ✅ Completed |
| ML-10 Content Action Playbook | w07_action_playbook.ipynb | ✅ Completed |
| ML-11 Capstone Research Paper | capstone.ipynb | ✅ Completed |
| ML-12 Demo, Social Post & Employer Summary | capstone.ipynb | ✅ Completed |

---

# Project Overview

This repository demonstrates an end-to-end machine learning workflow for identifying content improvement opportunities using anonymized SEO and engagement data.

The project includes:

- Research question definition
- ML task framing
- Data understanding and validation
- Feature engineering
- Feature leakage checks
- Baseline model evaluation
- Random Forest model development
- Grouped validation using client-based train/test split
- Content action recommendations
- Capstone research paper

---

# Final Model Performance

| Model | Accuracy |
|--------|---------:|
| Baseline (Dummy Classifier) | 0.7834 |
| Random Forest Classifier | 0.8382 |

The Random Forest model showed higher measured accuracy than the baseline on the grouped validation split. The results are observational and intended for decision support rather than guaranteed future performance.

---

# Responsible ML Practices

This project follows responsible machine learning principles.

- Results are reported as **observed** and **measured** outcomes.
- Findings are **directional** and intended for **decision support**.
- Human review is required before applying recommendations.
- No client-identifying or sensitive information is included.
- The model does not guarantee future content performance.

---

# Tools Used

- Python
- Pandas
- Scikit-learn
- Google Colab
- Git
- GitHub

---

# Repository Structure

```
work/
├── notebooks/
├── outputs/
├── figures/
├── scripts/
└── capstone_report.md
```

This repository contains all notebooks, outputs, and supporting files developed during the FlyRank Machine Learning Internship.
