# CMPE 256 Hotel Recommendation System

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
Neural Matrix Factorization  (NeuMF)
Singular value Decomposition (SVD) combined with sentiment analysis
Gradenet boost Machine (GBM) combined with sentiment analysis

## Folder Structure
```
cmpe256_hotel_recommendation_system/
│
├── data/
│   ├── raw/                      # Original, unprocessed dataset (if small enough)
│   └── processed/                # Cleaned & preprocessed data ready for modeling
├── notebooks/                   # Jupyter/Colab notebooks for EDA, model training, etc.
├── models/                      # Saved model files (e.g. .h5, .pkl, etc.)
├── src/                         # Source code modules (modularized functions/classes)
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


## How to Run
### 1. Clone the repository
`git clone https://github.com/Rodarkhen/cmpe256_hotel_recommendation_system.git`

### 2. Install Dependecies
Create a virtual environment (optional but highly recommended):

`python -m venv venv
source venv/bin/activate`

Then, install required Python packages with the following command:

`pip install -r requirements.txt`

