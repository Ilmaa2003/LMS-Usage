
# LMS Usage – Statistical Analysis Guide

A statistical research project examining the usage of a Learning Management System (LMS) based on survey or usage data. This guide outlines how to analyze the dataset using Microsoft Excel’s built-in **Data Analysis ToolPak**.

## Dataset

The Excel dataset used for this analysis is included in the project repository.

---

## 0. Enabling the Data Analysis ToolPak

Before performing any statistical analysis, ensure the **Data Analysis ToolPak** is activated:

1. Navigate to **File** → **Options**
2. Select **Add-ins**
3. At the bottom, under **Manage: Excel Add-ins**, click **Go**
4. Check the box labeled **Analysis ToolPak**
5. Click **OK**

Once enabled, the **Data Analysis** option will appear under the **Data** tab.

---

## 1. Descriptive Statistics

**Objective**: Provide summary statistics such as mean, median, standard deviation, etc., to understand the distribution of data.

**Steps**:

1. Go to **Data** → **Data Analysis**
2. Choose **Descriptive Statistics** and click **OK**
3. Configure:

   * **Input Range**: e.g., `A1:A50`
   * Enable **Labels in First Row** (if applicable)
   * Check **Summary Statistics**
4. Choose an output location and click **OK**

---

## 2. Correlation

**Objective**: Assess the degree of linear relationship between two variables.

**Steps**:

1. Open **Data Analysis** → Select **Correlation**
2. Configure:

   * **Input Range**: e.g., `A1:B50`
   * Enable **Labels in First Row**
   * Set grouping as **Columns**
3. Choose an output location and click **OK**

**Interpretation**:

* Value close to `+1`: Strong positive correlation
* Value close to `-1`: Strong negative correlation
* Value near `0`: No correlation

---

## 3. Regression Analysis

**Objective**: Evaluate how one or more independent variables influence a dependent variable.

**Steps**:

1. Go to **Data Analysis** → Select **Regression**
2. Configure:

   * **Input Y Range**: Dependent variable (e.g., `B1:B50`)
   * **Input X Range**: Independent variable(s) (e.g., `A1:A50`)
   * Enable **Labels** if headers are included
3. (Optional) Enable **Line Fit Plots** and set **Confidence Level**
4. Choose an output range and click **OK**

**Key Outputs**:

* **R Square (R²)**: Indicates the proportion of variance explained
* **P-values**: Test the significance of predictors
* **Coefficients**: Reflect the impact of each independent variable

---

## 4. T-Test

**Objective**: Compare the means of two groups to determine if the difference is statistically significant.

**Steps**:

1. Open **Data Analysis** → Select one of:

   * **t-Test: Two-Sample Assuming Equal Variances**
   * **t-Test: Two-Sample Assuming Unequal Variances**
2. Configure:

   * **Variable 1 Range**: e.g., `A1:A50`
   * **Variable 2 Range**: e.g., `B1:B50`
   * Enable **Labels** if applicable
3. Choose an output location and click **OK**

**Interpretation**:

* **P-value < 0.05**: Significant difference between group means
* **P-value ≥ 0.05**: No statistically significant difference

