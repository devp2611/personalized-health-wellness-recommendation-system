# Personalized Health & Wellness Recommendation System

A portfolio-ready data mining project that builds a personalized health and wellness recommendation system using Fitbit-based behavioral data such as daily activity, sleep, and heart rate.

## Project Overview

This project focuses on building a recommendation system using implicit user behavior rather than explicit ratings. The work combines multiple Fitbit-derived datasets into a unified daily-level dataset and analyzes user wellness patterns to recommend likely future behaviors.

The project includes:
- data merging and preprocessing
- exploratory data analysis
- implicit-feedback recommendation modeling
- evaluation using ranking-based metrics

## Problem Statement

Traditional recommender systems usually depend on explicit ratings. In contrast, wearable device data provides implicit signals such as recorded activity, sleep duration, and heart rate patterns. This project explores how those behavioral signals can be used to build a meaningful health and wellness recommendation system.

## Dataset Used

The project is based on Fitbit-derived data sources related to:
- daily physical activity
- sleep tracking
- heart rate tracking

These sources were merged into a final daily-level dataset for analysis and recommendation modeling.

## Methodology

The project was completed in the following stages:

### 1. Data Integration
Three health-related datasets were combined into a single structured dataset. Sleep data was aggregated to daily total sleep minutes, and heart rate data was aggregated to daily average BPM.

### 2. Data Preprocessing
The merged dataset was cleaned and standardized for modeling. Missing values were handled carefully to preserve the meaning of implicit interactions.

### 3. Exploratory Data Analysis
EDA was performed to understand user behavior patterns, activity distributions, sleep duration trends, and interaction sparsity.

### 4. Recommendation Models
The following recommendation approaches were implemented:
- Popularity Baseline
- Item-Item Collaborative Filtering
- Matrix Factorization (NMF)

### 5. Evaluation
Model performance was evaluated using:
- Precision@5
- Recall@5
- F1@5
- NDCG@5

## Key Findings

- The popularity-based recommendation model performed best on this dataset.
- User behavior patterns in the dataset were relatively homogeneous.
- Implicit behavioral data can support recommendation tasks, but careful interpretation is important.

## Repository Structure

```text
personalized-health-wellness-recommendation-system/
│
├── notebooks/
│   └── project.ipynb
│
├── data/
│   └── final_merged.csv
│
├── reports/
│   └── final_report.pdf
│
├── images/
│   └── project result images
│
└── README.md
