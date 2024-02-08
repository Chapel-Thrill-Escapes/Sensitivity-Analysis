# Price Sensitivity Analysis Project

## Overview

This project aims to analyze and visualize price sensitivity across different product categories. Utilizing R and the `ggplot2` library, the script processes four categories of price sensitivity data and generates a comprehensive plot that illustrates the cumulative percentage of respondents' price sensitivity.

## Installation

Before running the script, ensure you have R installed on your system. You will also need the `here` and `ggplot2` packages. If these are not already installed, the script will attempt to install `here` automatically.

## Usage

1. **Setting Up Your Environment**: The script utilizes the `here` package to set the working directory relative to the project root. This means you should have your project structured with the R script and the data files (`too_inexpensive_data.csv`, `inexpensive_data.csv`, `expensive_data.csv`, `too_expensive_data.csv`) in the same directory or a known structure that `here()` can recognize.

2. **Data Preparation**: The script reads in four CSV files representing different categories of price sensitivity:
   - Too Inexpensive
   - Inexpensive
   - Expensive
   - Too Expensive

   Each dataset should have at least two columns: `Price` and `Percent`, representing the price point and the percentage of respondents who rated it as such.

3. **Running the Script**: Execute the script in RStudio or your preferred R environment. The script will combine the data from the four categories, calculate cumulative sums for each, and plot the results.

4. **Viewing the Output**: The final output is a plot titled "Price Sensitivity Meter", which shows the cumulative percentage of respondents' sensitivity to different price points, categorized into four levels and color-coded for clarity.

## Plot Explanation

- **X-Axis (Price $)**: Represents different price points.
- **Y-Axis (% Respondents)**: Represents the cumulative percentage of respondents who have indicated a level of sensitivity (too inexpensive, inexpensive, expensive, too expensive) at or below each price point.
- **Colors**: Each category is represented by a different color for easy distinction.

## Requirements

- R
- `here` package
- `ggplot2` package

## Data Files

Place your data files in the project root or ensure they are accessible through the `here()` function. The expected files are:
- `too_inexpensive_data.csv`
- `inexpensive_data.csv`
- `expensive_data.csv`
- `too_expensive_data.csv`

Each file should follow the format of having at least `Price` and `Percent` columns.

