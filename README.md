# Budget Analysis and Optimization

## Overview

This project involves analyzing and optimizing the budget of a specific department. The dataset includes financial information for various departments, and the analysis focuses on identifying areas for potential cost savings and efficiency improvements.

## Dataset

The dataset pertains to the budgeting of a department and includes the following columns:

- **FISCAL YEAR**: The fiscal year for the data.
- **ALL FUNDS**: Total funds allocated to the department.
- **CITY FUND**: Funds actually spent by the department.
- **Variance**: Difference between `ALL FUNDS` and `CITY FUND`, indicating budget surplus or deficit.

## Analysis Performed

1. **Basic Analysis**:
   - Calculated total budget, actual spending, and total variance.

2. **Spending Patterns**:
   - Analyzed spending patterns across different fiscal years.

3. **Top Cost Savings Areas**:
   - Identified the top 10 areas with the highest variance between allocated funds and actual spending.

4. **Reallocation Suggestions**:
   - Provided example reallocation suggestions based on the variance data.

## Code

The analysis was performed using Python and the Pandas library. The key steps include:

1. **Calculate Variance**:
   ```python
   dept_df['Variance'] = dept_df['ALL FUNDS'] - dept_df['CITY FUND']
