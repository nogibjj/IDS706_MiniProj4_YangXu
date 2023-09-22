# IDS706_MiniProj4_YangXu

This repository is a continuation of the IDS706 course assignments, now focusing on Mini Project 4. Building upon the foundational work from previous assignments, this project introduces testing across multiple Python versions using GitHub Actions Matrix Build.

## Overview

In this project, we utilize GitHub Actions to perform continuous integration and deployment. The highlight of this project is the use of Matrix Build to test the code across multiple versions of Python on different OS environments.

## Key Modifications from Previous Assignments

- Introduced GitHub Actions Matrix Build in the `cicd.yml` file.
- Modified action workflow to test across Python 3.7, 3.8, and 3.9 on both `ubuntu-latest` and `ubuntu-20.04`.
- Retained the use of Pandas for data processing and visualization, as implemented in the prior assignment.

### Requirements

Ensure the presence of:
- Python (Version 3.7 or newer)
- Pandas (Refer to `requirements.txt` for exact version and other dependencies)

## Functionality

- **`load_data()`**: Imports the `dataset_sample.csv` and returns a DataFrame.

- **`get_descriptive_statistics(data)`**: Generates descriptive statistics from the DataFrame.

- **`plot_data_distribution(data, column_name)`**: Visualizes and saves a histogram for the specified column.

## Sample Output

- **Descriptive Statistics**:

    ```bash
          Price   Quantity
    count  9.000000   9.000000
    mean   1.433333  38.111111
    std    0.845577  14.084073
    min    0.500000  19.000000
    25%    0.700000  22.000000
    50%    1.200000  42.000000
    75%    2.400000  50.000000
    max    2.600000  55.000000
    ```

- **Data Visualization**:

  ![Price Distribution](Price_distribution.png)

### GitHub Actions Workflow

Test the code on multiple Python versions and OS environments using GitHub Actions Matrix Build.

[![GitHub Actions Workflow Status](https://github.com/nogibjj/IDS706_MiniProj4_YangXu/actions/workflows/cicd.yml/badge.svg)](https://github.com/nogibjj/IDS706_MiniProj4_YangXu/actions/workflows/cicd.yml)
