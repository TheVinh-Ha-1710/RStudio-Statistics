# RStudio Statistical Analysis Project

## Project Overview
This project involves conducting deep statistical analysis using RStudio on traffic and cake datasets. The study explores relationships between variables using regression models, evaluates model significance with statistical tests, and visualizes results using various plots. The project also includes a comprehensive study report created using RMarkdown.

## Datasets Used
- **Traffic Dataset**: Used to analyze relationships between different predictors and the response variable `spi`.
- **Cake Dataset**: Used for a two-way ANOVA study to examine the effects of `Recipe` and `Temp` on `Angle`.

## Key Analysis Steps
### **Traffic Dataset Analysis**
1. **Exploratory Data Analysis (EDA)**
   - Correlation analysis with correlation matrices and scatterplot matrices.
   - Identification of relationships between predictors and the response variable `spi`.

2. **Regression Model Fitting**
   - Full multiple linear regression model `lm(spi ~ ., data = traffic)`.
   - 95% confidence interval estimation for `weather` impact.
   - F-test for overall regression significance.

3. **Model Diagnostics**
   - Residual plots and normality tests.
   - Finding the best regression model through backward elimination.
   - Comparing adjusted R² values to determine optimal model selection.

### **Cake Dataset Analysis**
1. **Balanced Study Checking**
   - Ensuring equal number of replicates across factor levels.
   
2. **Preliminary Data Visualization**
   - Boxplots and interaction plots to analyze factor relationships.

3. **Two-Way ANOVA Analysis**
   - Interaction model fitting to assess significance.
   - Model validation through diagnostic plots.

4. **Main Effects Analysis**
   - Hypothesis testing for `Recipe` and `Temp` significance.
   - Final model selection without interaction term based on p-values.

## Tools & Libraries Used
- **RStudio** for data analysis and statistical modeling.
- **Base R functions** for data manipulation and visualization.
- **ggplot2 & Base R plotting functions** for visual representation.
- **RMarkdown** for creating a reproducible statistical report.

## Results & Findings
- A significant relationship was found between `spi` and predictors `weather`, `transport`, and `road` in the traffic dataset.
- The final regression model explained **73.8% of variation** in `spi`.
- The cake dataset analysis found that `Recipe` and `Temp` had significant main effects on `Angle`, but their interaction was not significant.

## How to Run the Project
1. Ensure R and RStudio are installed.
2. Place datasets (`traffic.csv`, `cake.csv`) inside the `data/` folder.
3. Open `report.Rmd` in RStudio.
4. Click **Knit** to generate the PDF report.
