# Flight Delay ML Pipeline

This project implements a complete data science pipeline to analyze and predict flight delays using historical flight data.
The pipeline covers exploratory data analysis, supervised learning, and unsupervised learning techniques.

---

## Quick Start

1. Create and activate a virtual environment:
```bash
python -m venv .venv
source .venv/bin/activate
.venv\Scripts\activate
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run the notebooks in order:
- 01_eda.ipynb
- 02_supervised_modeling.ipynb
- 03_unsupervised_modeling.ipynb

⚠️ Note: The repository includes a sampled dataset (flights_sample.csv) due to GitHub file size limitations.
To run the analysis with the full dataset, rename the file with flights.csv before running.

---

## Project Structure

- `data/`: Raw and processed datasets
- `notebooks/`: Jupyter notebooks for each project stage
  - `01_eda.ipynb`: Exploratory Data Analysis
  - `02_supervised_modeling.ipynb`: Supervised learning models
  - `03_unsupervised_modeling.ipynb`: Unsupervised learning analysis
- `src/`: Reserved for future modularization of preprocessing and feature engineering logic
- `requirements.txt`: Project dependencies

---

## Exploratory Data Analysis (EDA)

The exploratory analysis is available in the notebook below:

[Exploratory Data Analysis Notebook](notebooks/)

The EDA includes:
- Missing value analysis
- Delay rate analysis by airline and temporal features
- Visualizations highlighting daily and weekly delay patterns

---

## Environment

- Python version: **3.11.9**
- Main libraries: pandas, numpy, scikit-learn, matplotlib, seaborn

---

## Dataset

The original `flights.csv` dataset provided by the course contains over 5 million records and exceeds GitHub’s file size limits.
For this reason, a representative sample of the dataset (`flights_sample.csv`) is included in the repository and used throughout the analysis.

All notebooks are configured to load `flights.csv` by default, just change the name to run your project.

---

## Problem Definition

Flight delays cause significant operational and customer satisfaction issues in the aviation industry.
This project aims to analyze historical flight data to identify delay patterns and evaluate how well delays can be predicted using contextual and temporal flight information.

---

## Modeling Overview

The project applies both supervised and unsupervised machine learning techniques.

- **Supervised Learning**:  
  A binary classification task was defined to predict whether a flight is delayed by more than 15 minutes.
  Logistic Regression was used as a baseline model for interpretability, and Random Forest was applied to capture non-linear relationships.

- **Unsupervised Learning**:  
  Isolation Forest was used for anomaly detection to identify flights with extreme delay behavior, complementing the supervised analysis by highlighting rare and atypical events.

---

## Limitations and Future Work

The models rely exclusively on historical and contextual flight data and do not incorporate external factors such as weather conditions, real-time airport congestion, or aircraft availability.

As a result, predictive performance is limited for individual delay events.

Future improvements may include:
- Incorporating real-time or weather-related data
- Exploring regression models to predict delay duration
- Evaluating cost-sensitive learning or class imbalance techniques
- Deploying the model as an API or interactive dashboard
