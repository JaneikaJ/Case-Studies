# Individual Task 1: Case Studies — Part 1

EEG-based epileptic seizure detection using Random Forest and RBF-kernel Support
Vector Machine on two public datasets:

- **BEED** — Bangalore EEG Epilepsy Dataset (UCI Machine Learning Repository)
- **ESR** — Epileptic Seizure Recognition dataset (Kaggle)

## Repository structure

```
individual-task-1/
├── analysis.ipynb        # Full analysis notebook (preprocessing, modelling, evaluation)
├── README.md
└── results/
    └── figures/          # Confusion matrices, feature-importance and model-comparison plots
```

## Summary

- **Datasets analysed separately** — BEED (16 engineered channel summaries) and
  ESR (178 raw EEG time points) have different structures.
- **Models** — Random Forest (200 trees) and SVM (RBF kernel), both with balanced
  class weights, stratified 80/20 train–test split, scaler fitted on training only.
- **Metrics** — accuracy, balanced accuracy, precision, recall, F1-score, ROC-AUC
  and confusion matrices.
- **Key results (test set):**
  - BEED: RF 0.9975 accuracy / 0.9983 F1; SVM 0.9969 / 0.9979
  - ESR:  RF 0.9722 / 0.9276 F1; SVM 0.9752 / 0.9397 F1

## References

See `references.bib` in the assignment repository for the dataset, method and
context sources (UCI, Kaggle, Nicolaou & Georgiou 2012, Zhang et al. 2018,
Sharmila 2018, Alalayah et al. 2023, Andrzejak et al. 2001, Florey job ad).
