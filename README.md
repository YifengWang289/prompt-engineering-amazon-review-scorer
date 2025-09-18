# ⭐ Amazon Review Prediction with Prompt Engineering

## Overview
This project predicts **1–5 star review scores** from Amazon product reviews using **prompt engineering and NLP**.  
It addresses the common problem where reviews exist as free text without numerical ratings, making it difficult to compare products or track sentiment consistently.

## Business Value
- **Standardize review scores**: Convert unstructured reviews into a consistent 1–5 scale.  
- **Benchmark products**: Enable fair comparison across platforms even when ratings are missing.  
- **Support recommendation systems**: Provide additional signals for personalization and product ranking.

## AI Problem
- **Goal**: Predict review scores (1–5) from free-text reviews.  
- **Why NLP**: Requires semantic understanding of context, tone, and subtle language cues.  
- **Scalability**: Manual scoring isn’t feasible for millions of reviews — automation is essential.  

## 📊 Dataset
- 100 Amazon electronics reviews manually collected  
  - 20 reviews for each score (1–5)  
  - Includes review title & body  
- Balanced dataset ensures fair evaluation.  

## Methodology
1. Collect text reviews and star ratings.  
2. Apply **prompt engineering** to predict sentiment scores.  
3. Compare predicted ratings against ground truth.  
4. Evaluate using **MAE** and **RMSE**.  

## Results
- Demonstrated proof-of-concept on small dataset.  
- Prompt engineering achieved reasonable accuracy, with RMSE reflecting sensitivity to outliers.  
- Showcased potential for scalable integration into e-commerce platforms.  


## Tech Stack
- Python, Jupyter Notebook  
- Prompt Engineering (OpenAI / LLM-based approaches)  
- Pandas, NumPy for preprocessing  
- Matplotlib/Seaborn for visualization


[![Open In Colab]([https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/<你的ColabID](https://colab.research.google.com/drive/1t6Y6ykcb5Wub3ygAngEha7DTQbzRVxv0?usp=sharing)>)
