# Fine-Tuning BERT for Yelp Review Sentiment

This branch fine-tunes a BERT model for classifying Yelp reviews into 5 sentiment categories using the [Yelp Review Full dataset](https://huggingface.co/datasets/yelp_review_full).

## Steps
1. **Dataset**: Load and tokenize Yelp reviews.
2. **Model**: Use `bert-base-cased` with 5 output labels.
3. **Training**: Fine-tune using `Trainer` with evaluation per epoch.
4. **Evaluation**: Calculate accuracy on test data.

## Installation
```bash
pip install transformers datasets evaluate