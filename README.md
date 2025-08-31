# Synthetic Sales Data Analysis

This project is designed as a portfolio-ready example for roles such as Business Analyst, Program Manager, or Data Analyst. It includes a fully synthetic dataset, an analysis notebook with exploratory data visualizations and a simple predictive model, and the necessary configuration files to run everything out of the box.

## Project Overview

The objective of this project is to demonstrate how to perform end‑to‑end data analysis using a realistic, yet completely synthetic, sales dataset. The analysis covers:

- Loading and inspecting the dataset
- Exploratory data analysis (EDA) with descriptive statistics and visualizations
- Deriving insights, such as average revenue by region and product category
- Building a machine learning model to predict whether a sale qualifies as **high revenue**

By following this project, a potential employer can see your ability to work with tabular data, create compelling visuals, build predictive models, and document your work clearly.

## Dataset

The dataset is stored in **`synthetic_sales_data.csv`**. Each row represents a single sale. The fields include:

| Column            | Description                                         |
|------------------|-----------------------------------------------------|
| `Date`           | Date of the transaction                             |
| `Region`         | Geographical region (North, South, East, West)       |
| `Product_Category` | Type of product sold (Electronics, Furniture, Clothing, Food) |
| `Price`          | Price per unit (USD)                                |
| `Quantity`       | Number of units sold                                |
| `Customer_Age`   | Age of the customer                                 |
| `Satisfaction_Score` | Customer feedback rating (1–5)                 |
| `Product_Return` | Indicates whether the product was returned (0/1)    |
| `Revenue`        | Total revenue for the transaction (Price × Quantity) |

All data is synthetic and generated using random sampling. There is no personally identifiable information.

## Notebook

The **`sales_analysis.ipynb`** notebook walks through the analysis step by step:

1. **Introduction** – Brief overview of the problem and goals.
2. **Setup** – Importing libraries and loading the dataset.
3. **Exploratory Data Analysis** – Generating summary statistics and charts to understand the data.
4. **Predictive Modeling** – Creating a binary target variable for high revenue and training a logistic regression model.
5. **Conclusion** – Summarizing insights and model performance.

Run the notebook in any Jupyter environment to reproduce the analysis. Plots are generated using matplotlib and seaborn, and the model uses scikit‑learn.

## Requirements

Install the necessary Python packages with:

```bash
pip install -r requirements.txt
```

The key dependencies are:

- **pandas** – Data manipulation
- **numpy** – Numerical operations
- **matplotlib** and **seaborn** – Visualization
- **scikit‑learn** – Machine learning

A full list is provided in the `requirements.txt` file.

## Getting Started

1. **Clone or download** this repository.
2. Create a virtual environment (optional but recommended):

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Launch the notebook**:

   ```bash
   jupyter notebook sales_analysis.ipynb
   ```

5. Follow the cells in order. The dataset (`synthetic_sales_data.csv`) is loaded relative to the notebook, so no path modifications are necessary.

## Increasing Difficulty Extensions

To further challenge yourself and showcase more advanced skills, consider extending this project with:

- **Time Series Analysis** – Forecasting future sales using methods such as ARIMA or Prophet.
- **Segmentation** – Clustering customers or transactions to identify patterns and create personas.
- **Dashboarding** – Building an interactive dashboard using libraries like Plotly Dash or Tableau.
- **Model Tuning** – Experimenting with other algorithms (e.g., random forest, gradient boosting) and hyperparameter optimization.

## License

This project is released under the MIT License. You are free to use, modify, and distribute the code and data.
