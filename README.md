# CAFA-6 Protein Function Prediction

## What is this?

Predict what proteins do based on their amino acid sequences.

## Quick Start

### On Kaggle (easiest):
1. Go to the competition page
2. Click "Code" → "New Notebook"  
3. Copy your code and run it
4. Data is already there at `/kaggle/input/`

### Locally:
1. Install: `pip install pandas biopython`
2. Download data from Kaggle
3. Run: `jupyter notebook`

## The Goal

- **Input**: Protein sequences (like "MRWQEMGYIFYPRKLR...")
- **Output**: GO terms (like "GO:0000001") that describe what the protein does
- **Submit**: A TSV file with protein_id, GO_term, confidence

## Files

- `Train/train_sequences.fasta` - protein sequences to learn from
- `Train/train_terms.tsv` - which proteins have which GO terms
- `Test/testsuperset.fasta` - proteins you need to predict
- `sample_submission.tsv` - example of what to submit