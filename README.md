# Confidence-Based Review Analysis using NLP

This project explores the use of NLP models to understand how well user reviews on research papers align with their given confidence scores (rated 1 to 5).

---

## 📌 Objective

To investigate whether semantic similarity between research papers and user reviews (computed using NLP techniques) correlates with the users’ self-reported confidence scores.

---

## 🛠️ Models & Methods Used

We used the following techniques to compute similarity between a research paper and user review:

1. **BERT** - Pre-trained language model to capture deep contextual meaning.
2. **SciBERT** - A BERT variant trained on scientific texts for better domain-specific understanding.
3. **Jaccard Similarity** - A lexical-level comparison method based on set overlap.

All similarity scores were **scaled between 1 and 5** to match the scale of the original confidence scores.

---

## 📊 Results

| Model     | Correlation with Confidence Score |
|-----------|-----------------------------------|
| BERT      | -0.0376                           |
| Jaccard   | -0.0990                           |
| SciBERT   | -0.0523                           |

### 🔍 Inference

-The analysis revealed that semantic similarity alone may not be a strong predictor of user confidence in research paper reviews.

-Despite using both traditional (Jaccard) and advanced NLP models (BERT, SciBERT), the correlations with actual confidence scores remained weak.

-This highlights that user confidence is likely influenced by subjective factors such as prior knowledge, writing clarity, or perceived credibility, which are not fully captured through text similarity.
