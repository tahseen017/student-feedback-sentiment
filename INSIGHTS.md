# Insight memo — Coursera course reviews (107,018 reviews)

1. **Ratings are heavily skewed positive** — 74.0% of reviews are 5★ and 90.9% are 4–5★ (Chart 1). Only 4.4% are 1–2★, so the negative signal lives in a small but important tail.

2. **Machine sentiment tracks human stars** — Spearman r = 0.27 between VADER compound and the star rating, and mean compound rises monotonically 1★→5★ (Chart 4). VADER is a reliable automatic labeler here.

3. **Stars and text disagree on a notable minority** — 938 5★ reviews read negative (1.18% of 5★) and 756 1★ reviews read positive (30.62% of 1★); 3★ text averages +0.33, more positive than the middling star implies (Chart 4).

4. **What students praise:** top positive words/bigrams — 'great', 'good', 'really', 'well', 'learning', 'excellent', 'lot', 'thank'; phrases like 'machine learning', 'learned lot', 'easy understand', 'thank much', 'really enjoyed' (Charts 6 & 8). Teaching clarity and 'easy to follow' explanations dominate praise.

5. **What frustrates them:** top negative phrases — 'waste time', 'peer review', 'learned lot', 'machine learning', 'final project', 'difficult understand' (Charts 7 & 8); overall sentiment split: 89% positive / 6% neutral / 5% negative (Chart 5).

---
Method: NLTK VADER compound score on raw review text (±0.05 thresholds), Pearson/Spearman vs star rating, word clouds + bigram counts on cleaned text (lowercased, URLs/punctuation removed, stop-words filtered).