# CAFA-6 Protein Function Prediction

Baseline model using ESM2 embeddings and a linear classifier to predict GO terms for proteins.

## Model

- **Architecture**: Linear classifier (embedding → GO term probabilities)
- **Embeddings**: ESM2 (1280 dimensions)
- **Training**: BCEWithLogitsLoss, Adam optimizer, 3 epochs
- **Output**: Multi-label classification (25,980 GO terms)

## Files

- `first_model.ipynb` - Complete training and prediction pipeline
- `Train/train_terms.tsv` - Training labels
- `Test/testsuperset.fasta` - Test sequences
- `submission.tsv` - Generated predictions

## Usage

Works both locally and on Kaggle. The notebook automatically detects the environment and uses appropriate paths.

## Submission Format

TSV file with columns: `protein_id`, `GO_term`, `confidence` (no header)