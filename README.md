# Data Breach Chronology: Exploratory Data Analysis

This project explores data breaches reported across the United States using the [Privacy Rights Clearinghouse Data Breach Chronology](https://privacyrights.org/databreach) dataset.

## 📊 Project Objective

The goal is to provide an initial exploratory analysis that could support a potential client—such as a government agency or nonprofit cybersecurity organization—in identifying patterns and trends in public data breach reporting. This work is intended as a foundation for a larger, ongoing project that will evolve over time.

## 📁 Files Included

- `Exploratory Data Analysis of U.S. Data Breaches.qmd`: The Quarto document containing code and narrative
- `Exploratory Data Analysis of U.S. Data Breaches.html`: Rendered HTML output of the report
- `Data_Breach_Chronology_README.pdf`: Official dataset documentation from Privacy Rights Clearinghouse, detailing data sources, structure, and field definitions
- `README.md`: This file, containing project overview and instructions
- `Data_Breach_Chronology_sample.csv`: Sample version of the dataset in CSV format (for structural reference only)
- `Data_Breach_Chronology_sample.xlsx`: Sample version of the dataset in Excel format (for structural reference only)
- `Data_Breach_Chronology_sample.db`: SQLite version of the sample dataset (for structural reference only)

> ❗ **Note**: The dataset used for this project is not included due to licensing restrictions from the Privacy Rights Clearinghouse.

## 🔧 How to Reproduce

To reproduce this analysis, you must first obtain the dataset directly from the [Privacy Rights Clearinghouse](https://privacyrights.org/databreach) and agree to their terms of use.

Once the dataset is downloaded:

1. Save the dataset (in CSV format) in your working directory.
2. Ensure the column separator is `|` (pipe) when reading it into R.
3. Open `final_project_completed.qmd` in RStudio.
4. Render the Quarto file to generate your own version of the report.

### 🔢 Example code to load the dataset:

```r
data <- read.csv("Data_Breach_Chronology.csv", sep = "|")
```

## 📦 Requirements

- R (version 4.0 or higher)
- [Quarto](https://quarto.org/)
- RStudio (optional but recommended)
- No additional R packages required (base R is sufficient)

## 📌 Summary Insights

- **HACK-type breaches** are the most frequent and have the largest impact on individuals.
- **Healthcare and education sectors** are the most commonly targeted organization types.
- The distribution of breach sizes is **heavily skewed**, with a few large breaches affecting millions.
- Using **log-transformed histograms** provides a clearer picture of the true spread of breach sizes.

## 🚧 Ongoing Work

This project represents the beginning of a larger initiative to study U.S. data breaches. Planned next steps include:

- Time series analysis of breach frequency and impact over the years.
- Clustering breaches by type and size to reveal hidden groupings.
- Natural Language Processing (NLP) of breach notification letters for qualitative insights.

## 📝 Dataset Information

- **Source**: Privacy Rights Clearinghouse  
- **URL**: [https://privacyrights.org/databreach](https://privacyrights.org/databreach)  
- **License**: The dataset is not included in this repository due to licensing restrictions. Refer to [Terms of Use](https://privacyrights.org) for details on how to obtain and use the data responsibly.
