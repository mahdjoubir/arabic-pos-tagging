# PL-Score Implementation

This repository contains the implementation of the PL-Score, a complementary metric for evaluating POS-tagging errors in Arabic, as described in the paper "Relever les défis du TAL arabe via le POS-tagging avec une évaluation nuancée des transformers".

## Files
- `pl_score.py`: Python script to identify plausible errors and calculate the PL-Score.
- `example.txt`: Example input for testing the script.

## Usage
1. Install dependencies: `pip install camel-tools pandas`
2. Run the script: `python pl_score.py`
3. Replace the `buckwalter_lexicon` placeholder in `pl_score.py` with a real lexicon (e.g., from CAMeL Tools [Obeid et al., 2020]).

## Example
For the phrase "الكتاب الكبير", the script detects if NOUN→ADJ for "كبير" is a plausible error based on morphosyntactic rules.

## Notes
The rules are defined in Annexe 8.4 of the paper. This is a simplified implementation; contributions to expand the lexicon or rules are welcome!
