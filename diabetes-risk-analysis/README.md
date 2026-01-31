# Diabetes Risk Analysis

## Project Overview
This project analyzes diabetes risk using the CDC Diabetes Dataset. It follows the CRISP-DM methodology.

## Structure

- **data/**
  - `raw/`: The original CDC Diabetes Dataset.
  - `processed/`: The cleaned/balanced dataset.
- **notebooks/**
  - `01_eda_and_prep.ipynb`: Data Understanding & Preparation.
  - `02_clustering_analysis.ipynb`: Unsupervised Learning.
  - `03_classification_model.ipynb`: Supervised Learning & Evaluation.
- **models/**
  - Saved versions of trained models (.pkl or .joblib).
- **outputs/**
  - `figures/`: Saved plots, heatmaps, and ROC curves.

## Setup

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Run notebooks in order.
