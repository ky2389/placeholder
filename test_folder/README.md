# Data Analysis Project

## Introduction

Welcome to the Data Analysis Project! This assignment will test your skills in data manipulation, visualization, and analysis using Python. You'll be working with a real-world dataset to extract meaningful insights and present your findings.

## Project Requirements

### 1. Data Exploration and Cleaning

Before diving into analysis, you'll need to prepare your data:

- Load the dataset using pandas
- Check for missing values and handle them appropriately
- Identify and deal with outliers
- Perform necessary data transformations

### 2. Data Analysis

Perform the following analyses on the dataset:

- Calculate basic statistics (mean, median, standard deviation)
- Find correlations between variables
- Segment the data based on relevant criteria
- Test at least one hypothesis

### 3. Data Visualization

Create at least 4 different types of visualizations:

- A histogram or density plot
- A scatter plot showing relationships between variables
- A time-series plot (if applicable)
- A custom visualization of your choice

### 4. Conclusions and Recommendations

Based on your analysis:

- Summarize the key findings
- Provide actionable recommendations
- Discuss limitations of your analysis
- Suggest potential future work

## Code Examples

### Loading and Exploring Data

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

# Set style for plots
plt.style.use('seaborn-darkgrid')
sns.set_palette("deep")

# Load the dataset
df = pd.read_csv('customer_data.csv')

# Display basic information
print(f"Dataset shape: {df.shape}")
print("\nFirst 5 rows:")
print(df.head())

# Summary statistics
print("\nSummary statistics:")
print(df.describe())

# Check for missing values
print("\nMissing values per column:")
print(df.isnull().sum())
```


## Mathematical Formulas

The standard deviation (σ) is calculated as:

σ = √(Σ(x - μ)² / N)

Where:
- μ is the mean
- N is the number of data points

For clustering, we'll use the k-means algorithm which minimizes:

J = Σ Σ ||x_i^(j) - c_j||²

Where:
- x_i^(j) is the i-th data point in cluster j
- c_j is the center of cluster j


## Evaluation Criteria

| Component | Weight | Description |
|-----------|--------|-------------|
| Data Cleaning | 20% | Thoroughness and appropriateness of cleaning methods |
| Analysis | 30% | Depth and relevance of statistical analysis |
| Visualization | 25% | Quality and informativeness of visualizations |
| Conclusions | 15% | Validity and usefulness of findings |
| Code Quality | 10% | Organization, documentation, and efficiency |

![Data Analysis Process](./test_img.png)
