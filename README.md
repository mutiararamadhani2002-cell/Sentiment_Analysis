# 📊 Analyzing Media Coverage and Public Reaction to the Epstein File: Insights from X Data

> A sentiment analysis project by **TxT Group** for the Editorial Research and Strategy team of *The American Times*.

---

## 👥 Team Members

| Name |
|------|
| Rivaldi |
| Akbar Kanugraha |
| Indira Faisa Afgani |
| Mutiara Ayu Alzahra |

---

## 📌 Project Overview

This project analyzes public reactions to media coverage of the Epstein case on X (formerly Twitter). The goal is to help the Editorial Research and Strategy team understand public sentiment and key discussion themes, so that their reporting better reflects public concerns and ongoing discourse.

**Research Questions:**
1. How does the public respond to media coverage of the Epstein case on X?
2. What key concerns and discussion themes should the Editorial Research team highlight to ensure media coverage better represents public perspectives?

---

## 🗂️ Dataset

- **Source:** X (Twitter) — scraped using TweetHarvest (Python tool)
- **Period:** November 1, 2025 – March 12, 2026
- **Storage:** Raw data saved as `.csv` and uploaded to Google Cloud

### Dataset Columns

| Column | Description |
|--------|-------------|
| `id_str` | Unique identifier for each tweet |
| `created_at` | Timestamp of when the tweet was posted |
| `full_text` | The full content of the tweet |
| `retweet_count` | Number of retweets |
| `favorite_count` | Number of likes/hearts |
| `tweet_url` | Direct link to the tweet on X |

---

## ⚙️ Data Preprocessing Pipeline

1. **Text Cleaning** — Remove mentions, duplicates, hashtags, URLs, numbers, and punctuation
2. **Case Folding** — Convert all text to lowercase
3. **Tokenization** — Split text into individual words
4. **Slang Normalization** — Replace informal words with standard forms
5. **Words Filtering** — Remove stop words and dominant primary keywords
6. **Lemmatization** — Convert words to their base dictionary form
7. **Text Reconstruction** — Combine processed tokens into clean text
8. **Data Clean** — Upload to Cloud and ready to analyze

---

## 🔍 Sentiment Analysis Method

**Tool:** VADER (Valence Aware Dictionary and sEntiment Reasoner)

| Score Range | Category |
|-------------|----------|
| Score > 0.1 | Positive |
| -0.1 ≤ Score ≤ 0.1 | Neutral |
| Score ≤ -0.1 | Negative |

> VADER can detect sentiment across up to 7,500 words.

---

## 📈 Key Findings

### Sentiment Distribution
- 🔴 **Negative: 49.6%** — Widespread criticism and concern
- 🔵 **Positive: 25.6%** — Informative or affirmative engagement
- 🟡 **Neutral: 24.9%** — Primarily news sharing

### Top 10 Most Common Words
`evidence` · `document` · `people` · `war` · `like` · `investigation` · `time` · `iran` · `doj` · `child`

### Temporal Trend
Discussion volume remained relatively stable from November 2025 to February 2026, then **spiked sharply in March 2026**, likely triggered by new developments or increased media coverage.

### Overall Pattern
Public discourse reflects **moral outrage and systemic critique** rather than neutral deliberation, with frequent references to institutional bodies (DOJ), investigative processes, and documentation.

---

## ✅ Recommendations

### 1. Improve Transparency in Institutional Reporting
- Provide clear reporting on investigations, legal processes, and official developments
- Explain complex legal documents and evidence in a publicly accessible way
- Distinguish between verified information and unconfirmed claims on social media

### 2. Maintain a Victim-Centered Perspective
- Ensure media coverage remains victim-centered and respectful
- Provide updates on legal outcomes and victim advocacy efforts

---

## 🎨 Presentation

View the full project presentation on Canva:
https://canva.link/u31ptf2ffcv10v6

---

## 🛠️ Tools & Technologies

- **Scraping:** TweetHarvest (Python)
- **Storage:** Google Cloud
- **Sentiment Analysis:** VADER
- **Visualization:** Python (Matplotlib / WordCloud)

---

> *This project was developed as part of an academic/research exercise to support data-driven editorial decision-making.*
