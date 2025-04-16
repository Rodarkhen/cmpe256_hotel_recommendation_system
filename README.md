# Cmpe256 Hotel Recommendation System

## Objetive
Choosing the right hotel is often overwhelming due to the vast number of options and diverse user preferences. **Hotelic** is a personalized hotel recommendation system designed to help users make better decisions by analyzing user reviews, ratings, and metadata using advanced recommender system techniques.

This project is developed as part of the CMPE 256 Project.

## Team
**Team Name**: Hotelic

**Members**
- Rodrigo Chen
- Anthony Luu
- Henry Nguyen


## Project Overview
We used the HotelRec dataset from TripAdvisor. It contains over 50 million reviews, which is well suited to develop an hotel recommender system based on the user interaction and behaviors towards the hotels.

The goal of this project is to create an efficient and reliable recommender system.

## Algorithms Used


## Folder Structure
```
cmpe256_hotel_recommendation_system/
│
├── data/
│   ├── raw/                      # Original, unprocessed dataset (if small enough)
│   └── processed/                # Cleaned & preprocessed data ready for modeling
│
├── notebooks/                   # Jupyter/Colab notebooks for EDA, model training, etc.
│   ├── 01_eda.ipynb             # Exploratory data analysis
│   ├── 02_preprocessing.ipynb   # Data cleaning & feature engineering
│   ├── 03_neumf_model.ipynb     # NeuMF model training
│   ├── 04_sentiment_model.ipynb # Sentiment-aware recommender
│   └── 05_clustering_model.ipynb# Clustering recommender
│
├── models/                      # Saved model files (e.g. .h5, .pkl, etc.)
│   ├── neumf_model.h5
│   └── sentiment_model.pkl
│
├── src/                         # Source code modules (modularized functions/classes)
│   ├── __init__.py
│   ├── data_loader.py           # Functions to load and preprocess data
│   ├── feature_engineering.py   # Feature extraction logic
│   ├── sentiment_analysis.py    # Sentiment/aspect extraction functions
│   ├── model_neumf.py           # NeuMF model definition
│   ├── model_sentiment.py       # Sentiment-aware model definition
│   └── model_clustering.py      # Clustering logic
│
├── outputs/                     # Results like graphs, evaluation reports, metrics
│   ├── plots/
│   └── metrics/
│
├── report/                      # Final report and presentation
│   ├── Hotelic_Report.pdf
│   └── Hotelic_Presentation.pptx
│
├── requirements.txt             # Python dependencies
├── README.md                    # Project overview and instructions
└── .gitignore                   # Files to ignore (e.g., dataset, model files)
```

## Git Workflow & Commit Message Convention

### Branching Strategy

- `main`: Stable and production-ready code.

- `feature/{jira-issue-name}`: New features are developed here before merging into develop.

- `bugfix/{jira-issue-name}`: Fixes for bugs found in develop.

- `hotfix/{jira-issue-name}`: Urgent bug fixes that need to be patched into main.

### Commit Message Format

To maintain consistency and readability, we follow this structured format:
```
[type]: [short description]

[Optional detailed description]
```

**Commit Types**:
- `feat`: A new feature
- `fix`: A bug fix
- `docs`: Documentation updates
- `refactor`: Code restructuring without functionality changes
- `chore`: Maintenance tasks (build processes, dependency updates, etc.)