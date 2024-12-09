# Wildfire Risk Analysis and Association Rule Mining

This project focuses on analyzing wildfire data to extract meaningful insights and patterns using machine learning models and association rule mining techniques. The aim is to understand wildfire causes, sizes, and seasonal patterns, ultimately contributing to risk prediction and management.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Data](#data)
- [Analysis and Models](#analysis-and-models)
- [Results](#results)
- [Future Work and Improvements](#future-work-and-improvements)
- [Requirements](#requirements)
- [Usage](#usage)

## Overview
Wildfires pose a significant environmental and economic threat. This project leverages wildfire data to identify relationships between factors such as fire size, cause classification, and discovery season. The project applies machine learning models, including Gradient Boosting and Random Forest, and association rule mining to understand wildfire behavior and patterns.

## Features
1. **Hierarchical Clustering**:
   - Identifies clusters in wildfire data based on numerical attributes.
   - Visualized using dendrograms to determine optimal clusters.

2. **Machine Learning Models**:
   - **Gradient Boosting Regressor** and **Random Forest Regressor**:
     - Predicts target variables (e.g., fire size or discovery season).
     - Evaluates model performance using scatter plots of actual vs. predicted values.
     - Extracts and visualizes feature importances.

3. **Association Rule Mining**:
   - Identifies rules linking fire causes, sizes, and discovery seasons.
   - Metrics include support, confidence, lift, and conviction for rule evaluation.

4. **Visualization**:
   - Scatter plots and bar plots for model evaluation and feature importance.
   - Dendrograms for clustering.

## Data
The dataset includes attributes related to wildfires, such as:
- **FIRE_SIZE_CLASS**: Size category of the fire.
- **NWCG_CAUSE_CLASSIFICATION**: Cause of the fire (e.g., Natural, Human).
- **DISCOVERY_SEASON**: Season when the fire was discovered.

## Analysis and Models
### Association Rule Mining
For example:
- **Rule 1**: If a fire is caused by natural factors (`NWCG_CAUSE_CLASSIFICATION_Natural`), there is a 43.3% probability it will be discovered in the summer (`DISCOVERY_SEASON_Summer`) with a fire size of 0 to 0.25 acres. The lift of 2.632 indicates this relationship is more than twice as likely as expected by chance.

### Machine Learning
Models used:
- **Gradient Boosting Regressor**: Predicted fire characteristics with significant accuracy. Features like cause classification and fire size were most influential.
- **Random Forest Regressor**: Provided robust predictions with insights into feature importances.

## Results
- **Clustering**: Revealed distinct groups in wildfire data based on geographical and temporal features.
- **Association Rules**: Strong patterns identified, such as natural causes correlating with small fires in the summer.
- **Model Accuracy**: Both Gradient Boosting and Random Forest achieved high prediction accuracy, with feature importance analyses highlighting key contributors like fire size and discovery season.

## Future Work and Improvements
1. **Expand Data Coverage**:
   - Incorporate real-time data for dynamic analysis.
   - Include additional features such as meteorological data or vegetation indices.

2. **Model Deployment**:
   - Develop a user-friendly web-based dashboard to visualize predictions and insights.
   - Deploy predictive models for real-time wildfire risk assessment and alerts.

3. **Optimization**:
   - Experiment with advanced models like XGBoost and deep learning.
   - Optimize clustering methods to enhance interpretability.

4. **Interactive Features**:
   - Implement interactive visualizations for better stakeholder engagement.

## Requirements
- Python 3.8 or later
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`, `scipy`, `mlxtend`

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/wildfire-Prediction-.git
   cd wildfire-Prediction-
