N-gram Language Models

This project implements unigram, bigram, and trigram language models on a large English news corpus to study how context size, smoothing, and sampling strategies affect perplexity and generated text quality.

Features

- Builds unigram, bigram, and trigram models with START/STOP sentence padding.
- Computes train and test perplexity with and without Laplace (add‑one) smoothing.
- Shows how Laplace smoothing can severely degrade higher‑order n‑gram performance on large vocabularies.
- Generates sample sentences using greedy decoding, random sampling, and top‑p (nucleus) sampling for each n‑gram order.

Files

- N gram Language model.ipynb: notebook for training models, computing perplexity, and generating text.
- HW4-Ngrams-2224541.pdf: report describing the modeling approach, perplexity results, and qualitative analysis of generated outputs.

How to Run

1. Place 1bbenchmark.train.tokens and 1bbenchmark.test.tokens where the notebook expects them, or update the trainfile and testfile paths.
2. Open N gram Language model.ipynb in Jupyter or Colab.
3. Run all cells to:
   - Load and preprocess data.
   - Build unigram, bigram, and trigram models.
   - Print the perplexity table (unsmoothed vs Laplace).
   - Generate sample sentences with different decoding strategies.

Takeaways

This project illustrates how classic n‑gram language models are built and evaluated, why naive add‑one smoothing is problematic for higher‑order models, and how decoding choices (greedy vs random vs top‑p) influence fluency and diversity in generated text.
