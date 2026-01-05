# Flight Delay ML Pipeline

This project implements a complete data science pipeline to analyze and predict flight delays using historical flight data.
The pipeline covers exploratory data analysis, supervised learning, and unsupervised learning techniques.

## Project Structure

- `data/`: Raw and processed datasets
- `notebooks/`: Jupyter notebooks for each project stage
  - `01_eda.ipynb`: Exploratory Data Analysis
  - `02_supervised_modeling.ipynb`: Supervised learning models
  - `03_unsupervised_modeling.ipynb`: Unsupervised learning analysis
- `src/`: Helper modules for preprocessing and feature engineering
- `figures/`: Generated visualizations
- `requirements.txt`: Project dependencies

## Exploratory Data Analysis (EDA)

The exploratory analysis is available in the notebook below:

[Exploratory Data Analysis Notebook](notebooks/01_eda.ipynb)

The EDA includes:
- Missing value analysis
- Delay rate analysis by airline and temporal features
- Visualizations highlighting daily and weekly delay patterns

## Environment

- Python version: **3.11.9**
- Main libraries: pandas, numpy, scikit-learn, matplotlib, seaborn

## Dataset

The original `flights.csv` dataset provided by the course contains over 5 million records and exceeds GitHub’s file size limits.
For this reason, a representative sample of the dataset (`flights_sample.csv`) is included in the repository and used throughout the analysis.

All notebooks are configured to load `flights.csv` by default, just change the name to run your project.
