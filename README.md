# Predict New Medicines with BELKA
### Kaggle Competition: Public LB Top 8%, Private LB Top 12%
Focused on drug discovery by predicting molecular properties using transformer-based models and 1D-CNN models.

## Key Features
- SMILES tokenization and sequence modeling.
- Transformers and CNN hybrid models.
- Rigorous cross-validation for robustness.

## Chanllenge
1. Unseen Data in Private Leaderboard:
The private leaderboard introduced molecular structures (building blocks) absent from both training and public validation datasets.
This led to a significant leaderboard shakeup, highlighting the difficulty of generalization.
2.Overfitting:
Public leaderboard performance did not always align with private leaderboard results, emphasizing the challenge of generalizing to unseen data.

## Key Takeaways

-Transformer Generalization:
Transformers, when lightly fine-tuned, excelled at generalizing to unseen datasets. Overfitting during fine-tuning impaired their ability to predict novel data.
-Fine-Tuned ChemBERTa:
Specialized fine-tuning on ChemBERTa for unseen data improved private leaderboard performance over traditional overfitting-prone models.
-Simplicity Wins:
Simple 1D-CNN architectures paired with basic SMILES tokenization often outperformed complex approaches.

## Insights
Can models truly generalize to unseen data in real-world, complex biological scenarios?
This competition raises concerns about model reliability in such cases, underscoring the need for further research.

## Data
Data can be accessed on [Kaggle BELKA Dataset](https://www.kaggle.com/c/neurips-2024-predict-new-medicines/data).
