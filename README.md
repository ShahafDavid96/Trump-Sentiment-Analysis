# Sentiment Analysis of Trump-Related Discourse Across Political Subreddits

## Project Overview

This repository contains code and analysis for our study examining sentiment toward Donald Trump across different political communities on Reddit. The project investigates how sentiment varies across subreddits of different political orientations, comparing patterns between post titles and comments, and tracking sentiment changes in response to significant political events.

## Key Features

- **Multi-method content identification**: Implementation of a robust approach to identify Trump-related content using direct keyword matching, named entity recognition, co-occurrence analysis, and pronoun pattern detection.

- **Advanced sentiment analysis**: Application of RoBERTa transformer-based models to capture nuanced sentiment expressions in political text, overcoming limitations of traditional lexicon-based approaches.

- **Comparative analysis**: Examination of sentiment patterns across Conservative, Liberal, and Centrist subreddits, revealing unexpected similarities and differences in how Trump is discussed.

- **Temporal trend analysis**: Tracking of sentiment changes in response to major political events during the 2024-2025 period, including presidential debates, election outcomes, and other significant moments.

- **Lexical analysis**: Word frequency and pattern analysis showing distinct vocabulary distributions across positive, neutral, and negative content.

## Major Findings

- Sentiment toward Trump is predominantly negative across all political orientations, with variation primarily in the degree of negativity rather than in positive sentiment expression.

- A consistent "sentiment gap" exists between post titles and comments, with comments displaying substantially higher negative sentiment across all community types.

- Conservative subreddits exhibit greater sentiment reactivity to political events compared to Liberal communities, which maintain more stable negative sentiment regardless of external developments.

- Lexical analysis reveals distinct discourse patterns across sentiment categories: positive content mirrors Trump's rhetorical style, neutral content focuses on institutional aspects, and negative content employs critical framing.

# Repository Structure

This repository contains two main Jupyter notebooks:

## 1. sentiment.ipynb

The primary analysis notebook containing the complete pipeline for sentiment analysis of Trump-related content across political subreddits. This notebook includes:

- Data loading and exploration
- Text preprocessing and cleaning
- Trump-related content identification using multi-method approach
- RoBERTa sentiment analysis implementation
- Cross-subreddit comparative analysis
- Temporal trend visualization and analysis
- Lexical pattern analysis with word clouds and frequency distributions
- Visualization of results and statistical analysis
## 2. downloader.ipynb

A data preparation utility notebook that:

- Converts JSONL files (from Reddit API data collection) to structured dataframes
- Merges multiple JSONL files from different political subreddits
- Exports a single merged CSV file (`merged_posts.csv` and `merged_comments.csv`)

Run this notebook first to prepare the dataset for the main analysis. The resulting merged CSV files serve as input for the `sentiment.ipynb` notebook.

