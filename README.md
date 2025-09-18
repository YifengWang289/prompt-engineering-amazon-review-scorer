# Amazon Review Rating Prediction

## Overview
Consumers often write product reviews in free text without giving a star rating.  
This makes it difficult for platforms and businesses to measure sentiment, compare products, or track customer satisfaction consistently.  

This project explores how free-text reviews can be **mapped into 1–5 star ratings** using prompt-based natural language processing (NLP). The goal is to demonstrate how carefully designed prompts can turn unstructured text into structured scores.

## Business Problem
- Many reviews lack a numeric rating, leaving only text.  
- Platforms cannot easily compare products or track sentiment across sites when ratings are missing or inconsistent.  
- Manual scoring of reviews is too slow and costly at scale.

## Business Value
- **Standardization:** Convert free-text reviews into a consistent 1–5 scale.  
- **Coverage:** Extend rating signals to places where only text exists (forums, social media, video comments).  
- **Decision support:** Help platforms and sellers benchmark products and understand customer sentiment more clearly.

**Who benefits?**
- **E-commerce platforms & sellers:** Gain structured insights for product evaluation.  
- **Consumers:** See more consistent ratings even when only text feedback is provided.

## Project Goal
Predict the **1–5 star rating** of a review of en electronic product based on its text using prompt engineering.  
The focus is on testing whether large language models can interpret tone, context, and wording well enough to approximate structured scores.

## Methodology
1. **Data:** 100 balanced Amazon electronics reviews with rating score (20 per rating from 1–5).  
2. **Prompt design:** Created a clear 1–5 rubric (very negative → very positive).  
3. **LLM inference:** Supplied review text to an LLM with structured instructions.  
4. **Post-processing:** Parsed predicted ratings from LLM output.  
5. **Evaluation:** Compared predictions against ground-truth labels.

## Evaluation
- Metrics: **Mean Absolute Error (MAE)** and **Root Mean Squared Error (RMSE)**.  
- Results: Predictions were on average within **one star** of the true rating (MAE ~0.7–1.0).  
- **Extreme ratings (1 and 5 stars)** were most reliable — strong positive/negative wording is easier to classify.  
- **Mid-range ratings (2–4 stars)** were more challenging due to mixed opinions and ambiguity.  

## Limitations
- Small dataset (100 reviews).  
- Restricted to electronics; not generalize across product categories.  
- Performance is sensitive to prompt wording.  
- Subjectivity remains in borderline/mixed reviews.

## Future Work
- Expand dataset to thousands of reviews across categories.  
- Experiment with few-shot prompting for better consistency.  
- Benchmark against classical ML and fine-tuned NLP models.  
- Combine text-based predictions with structured product attributes.



