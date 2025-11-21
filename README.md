# Diabetes Prediction & Regression Analysis

![R](https://img.shields.io/badge/R-4.2.3+-blue.svg)
![caret](https://img.shields.io/badge/caret-6.0+-orange.svg)
![tidyverse](https://img.shields.io/badge/tidyverse-2.0.0+-blueviolet.svg)
![ggplot2](https://img.shields.io/badge/ggplot2-3.4.2+-green.svg)


This project performs a comprehensive analysis of a balanced dataset (50-50 diabetic vs. non-diabetic) to predict health outcomes. It utilizes various statistical and machine learning techniques in R to identify key health indicators and compare the performance of multiple classification models.

## Description

The project is structured to handle data cleaning, exploratory data analysis (EDA), feature selection, and model training. The primary goal is to decrease bias using a balanced dataset and accurately predict `Diabetes_binary` status. Following prediction, the project focuses on inference using Decision Trees to create interpretable health rules.

## Features

* **Data Preprocessing:** Handling of duplicates and NA values to ensure dataset integrity.
* **Exploratory Data Analysis (EDA):** Visualization of relationships between diabetes and factors like BMI, Blood Pressure, Cholesterol, and Income using `ggplot2`.
* **Feature Selection:** Implementation of Forward and Backward Stepwise selection (using AIC) to identify the top 5 predictive features.
* **Model Comparison:** Training and evaluation of 8 different algorithms using 5-fold Cross-Validation:
    * QDA & LDA
    * Random Forest (`rf`)
    * Neural Network (`nnet`)
    * Conditional Inference Tree (`ctree`)
    * Linear SVM
    * Logistic Regression (`LogitBoost`)
    * K-Nearest Neighbors (`knn`)
* **Inference:** Pruned Decision Tree generation for interpreting the logical flow of diagnosis.

## Installation

1.  Ensure you have **R** installed (version 4.2+ recommended).
2.  Clone this repository.
3.  Install the required dependencies by running the following command in your R console:

```r
install.packages(c("caret", "pROC", "ggplot2", "tidyverse", "leaps", "MASS", "tree"))
````

## Usage

1.  **Prepare Data:**
    Ensure your dataset (e.g., `d2.csv`) is placed in the `Data/` directory.
    *Note: You may need to update the file path in `HW2.R` or `HW2-Code.Rmd` line: `read.csv("path/to/your/d2.csv")`.*

2.  **Run Analysis:**
    You can run the raw script or knit the R Markdown file for a report.

    ```r
    # Run the main script
    source("HW2.R")
    ```

    Or open `HW2-Code.Rmd` in RStudio and click **Knit** to generate an HTML/PDF report.

## Contributing

Contributions are welcome\!

1.  Fork the repository.
2.  Create a feature branch (`git checkout -b feature/NewModel`).
3.  Commit your changes.
4.  Push to the branch and open a Pull Request.

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Contact

**Nima Kelidari**
Project Link: [https://github.com/nikelroid/regression-hw2](https://www.google.com/search?q=https://github.com/nikelroid/regression-hw2)
