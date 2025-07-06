# QuitBit

## Project Objective
This project aims to predict employee turnover (i.e., whether an employee will stay or quit) using machine learning algorithms, specifically Decision Trees and Random Forests. The model assists HR departments in identifying employees at risk of attrition based on key behavioral and demographic features.

## Dataset Overview
The dataset contains records of employees, including:

- Categorical Features: Department, Salary level

- Numerical Features: Performance evaluation, average monthly hours, time spent at the company

- Target Variable: Whether the employee quit (1) or stayed (0)

## Project Workflow
1. Data Preprocessing & Cleaning
- Loaded CSV data using pandas

- Converted categorical variables (department, salary) into numeric form using one-hot encoding

- Removed redundant columns post-encoding

2. Exploratory Data Analysis (EDA)
- Visualized salary distribution vs. turnover frequency

- Checked class imbalance using Yellowbrick's ClassBalance visualizer

3. Train-Test Split
- Performed an 80/20 split using stratified sampling to preserve target distribution

4. Model Building
- Built an interactive Decision Tree Classifier with tunable hyperparameters using ipywidgets

- Built an interactive Random Forest Classifier with UI sliders for model customization

- Displayed visual tree structure using Graphviz within the notebook

5. Model Evaluation
- Computed accuracy on training and testing data

- Used Yellowbrick visualizers for:

    - Feature Importance

    - ROC-AUC Curves

## Key Features
- Interactive Tuning: Change model parameters using sliders without modifying code

- Visual Decision Trees: Graphical representation of classification logic

- Performance Metrics: Easily interpreted evaluation plots (ROC, importance, class balance)

- Explainability: Feature importance insights help identify what factors influence employee decisions

## Sample Outputs
- Turnover distribution bar graph

- Decision tree diagram for selected parameters

- Random forest sample tree visualization

- Feature ranking via bar chart

- ROC-AUC comparison between Decision Tree and Random Forest

## Tools & Libraries
- pandas, numpy — data manipulation

- matplotlib, yellowbrick — plotting and visual analytics

- scikit-learn — ML models and evaluation

- ipywidgets, graphviz, IPython.display — interactivity and visualization

- pandas_profiling — automated EDA (optional step)

## Conclusion
This project provides a full machine learning pipeline for understanding and predicting employee attrition. The use of tree-based models not only delivers strong performance but also maintains interpretability — a key requirement in HR applications.