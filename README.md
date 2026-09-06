# Customer Shopping Trends – Data Visualization Project

## Introduction

This project explores customer shopping behaviour using a synthetic Indian retail dataset containing 10,000 transactions.

The main goal was not simply to create charts, but to use visualizations to answer meaningful questions about customer behaviour, product performance, promotions, online and offline shopping, discounts, delivery, ratings, and returns.

The project includes data preparation, hypothesis-driven exploratory analysis, saved figures and tables, and a two-page interactive Power BI dashboard.

- [View the notebooks](notebooks/)
- [View the Power BI dashboard](dashboard/customer_shopping_trends_dashboard.pbix)
- [View the dataset on Kaggle](https://www.kaggle.com/datasets/rewantbhriguvanshi/customer-shopping-trends-indian)

## Background

This project was developed as part of my Data Analytics internship at CodeAlpha.

The task focused on transforming raw data into useful charts, graphs, and dashboards that make patterns easier to understand and support decision-making.

For this project, I used the **Customer Shopping Trends Indian Dataset**, a synthetic retail dataset representing customer transactions across different products, brands, cities, shopping channels, payment methods, promotions, delivery conditions, ratings, and returns.

Because the dataset is synthetic, the findings in this project describe patterns within the simulated transactions and should not be treated as conclusions about all Indian consumers or any real company.

## Dataset Overview

The original dataset contains:

- **10,000 transactions**
- **26 original columns**
- **3,291 unique customers**
- transactions from **January 2023 to December 2024**
- no missing values
- no exact duplicate rows
- unique transaction IDs

The dataset covers three main product categories:

- Clothing
- Footwear
- Accessories

It also includes information related to:

- customer demographics
- brands and products
- purchase amount and quantity
- discounts and promotional sales
- online and offline shopping
- payment methods
- subscriptions
- shipping charges
- delivery time
- ratings
- product returns

During data preparation, additional fields were created for analysis, bringing the processed dataset to **40 columns**.

## Tools and Libraries Used

- **Python** – main language used for data preparation and analysis
- **Pandas** – data cleaning, transformation, grouping, and aggregation
- **NumPy** – numerical operations
- **Matplotlib** – creation of charts and visualizations
- **Jupyter Notebook** – development and documentation of the analysis
- **Power BI** – creation of the final interactive dashboard

The required Python dependencies are listed in [`requirements.txt`](requirements.txt).

To install them:

```bash
pip install -r requirements.txt
```

## Project Structure

```text
Customer_Shopping_Trends_Viz/
│
├── data/
│   ├── customer_shopping_behavior.csv
│   └── processed_customer_shopping_behavior.csv
│
├── notebooks/
│   ├── 01_data_inspection_and_preparation.ipynb
│   └── 02_exploratory_visual_analysis.ipynb
│
├── dashboard/
│   ├── customer_shopping_trends_dashboard.pbix
│   └── Screenshots/
│
├── outputs/
│   ├── figures/
│   └── tables/
│
├── requirements.txt
├── .gitignore
└── README.md
```


## Project Workflow

The project follows a simple analysis pipeline:

**Raw Dataset → Data Inspection & Preparation → Processed Dataset → Exploratory Visual Analysis → Exported Figures & Tables → Power BI Dashboard → Business Insights**

### 1. Data Inspection and Preparation

The first notebook checks the structure and quality of the dataset, validates the main fields, creates analysis-friendly features, and saves the processed dataset.

### 2. Exploratory Visual Analysis

The second notebook uses six hypotheses to investigate promotions, customer groups, product performance, shopping channels, discounts, and customer experience.

The analysis produces 29 final visualizations and 30 supporting tables.

### 3. Power BI Dashboard

The processed dataset is then used to create a two-page interactive Power BI report:

- **Overview & Sales Performance**
- **Customer Experience & Returns**

The dashboard provides an interactive summary of the main findings using slicers, KPI cards, trend charts, category comparisons, and customer-experience analysis.

[View Dashboard Screenshots](dashboard/Screenshots/)

## Closing Thought

- This was a fun project to work on, especially since the dataset was already fairly clean.
- Creating the dashboard was probably the best experience for me once I had a clear plan for it.
- I was also glad to see that at least one of my hypotheses was fully supported by the data.
- If you want to approach data visualization as an analysis rather than just creating charts, I strongly recommend the hypothesis structure I used:

```text
1. Question — what the analysis is trying to determine;
2. Hypothesis — the expected pattern before examining the results;
3. Measures — the variables and calculations used;
4. Visual Analysis — charts used to examine the pattern;
5. Findings — observations directly supported by the results;
6. Verdict — whether the hypothesis was supported, partially supported, or not supported.
```

I had previously studied statistical hypothesis testing in college, where we used a somewhat similar structure for problem-solving. That gave me the idea to organize the visual analysis this way.

For the complete findings and conclusions, refer to Notebook 2.

[View Notebook 2](notebooks/02_exploratory_visual_analysis.ipynb)