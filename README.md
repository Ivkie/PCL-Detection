# Natural Language Processing: Patronising and Condescending Language Detection

Binary classification of patronising and condescending language (PCL) in English text, following the original the SemEval-2022 Task 4 benchmark.

## Overview

Subtle condescension in text is notoriously hard to detect — it often hides behind polite framing, charitable wording, or performative empathy.

```
├── BestModel/          # Final model code + prediction outputs
│   ├── model.ipynb     # Training pipeline
│   ├── dev.txt         # Dev set predictions
│   └── test.txt        # Test set predictions
├── data/               # Dataset loading and preprocessing scripts
└── README.md
```

## Model

Fine-tuned transformer classifier trained on the [Don't Patronize Me!](https://github.com/Perez-AlmendrosC/dontpatronizeme) dataset. Evaluated using F₁ on the positive (PCL) class against the SemEval-2022 Task 4 official leaderboard.

## Dataset

Perez-Almendros et al. (2022) — *SemEval-2022 Task 4: Patronizing and Condescending Language Detection*, ACL Anthology.
