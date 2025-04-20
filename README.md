# 🧠 Paper Review Confidence Scorer using NLP

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

- All models showed **negative correlation** with actual confidence scores.
- This suggests that user confidence may depend on **more subjective or external factors**, not just semantic similarity.
- Simple models like Jaccard performed worse, while even advanced models like BERT/SciBERT didn’t show meaningful positive correlation.



