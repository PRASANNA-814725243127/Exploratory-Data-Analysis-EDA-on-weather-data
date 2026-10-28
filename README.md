# Exploratory Data Analysis of Weather Data

A beginner-friendly Python project that demonstrates **Exploratory Data Analysis (EDA)** on weather data using Google Colab, Pandas, NumPy, Matplotlib, and Seaborn.

## Project Overview

This project creates a sample weather dataset containing 30 daily records, introduces missing values, inspects the raw data, cleans the dataset, calculates descriptive statistics, and visualizes patterns in weather measurements.

> **Dataset note:** The notebook generates synthetic/sample weather data for demonstration. It does not represent official observations from a weather station.

## Objectives

- Inspect dataset structure, data types, missing values, and duplicate rows.
- Handle missing numeric values using each column's median.
- Convert weather categories into numeric codes for analysis.
- Summarize numerical features using descriptive statistics.
- Explore weather patterns through five visualizations.

## Tools and Libraries

- Python
- Google Colab / Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Excel files (`.xlsx`) for saving the raw and cleaned datasets

## Project Files

```text
weather-eda-github/
├── README.md
├── Weather_EDA_Colab.ipynb
└── assets/
    └── github-upload-guide.jpeg
```

The notebook creates these files when its cells are run:

- `messy_weather_data.xlsx` — sample raw dataset with missing values.
- `cleaned_weather_data.xlsx` — dataset after the cleaning steps.

## Workflow

1. **Import libraries** — load NumPy, Pandas, Matplotlib, and Seaborn.
2. **Create sample data** — generate 30 daily records with weather features and some missing values.
3. **Inspect the data** — check dimensions, column types, missing values, and duplicate rows.
4. **Clean the data** — fill missing values in `Temperature`, `Humidity`, `Wind_Speed`, and `Visibility` with their column medians. Encode `Weather_Type` as `Sunny = 0`, `Cloudy = 1`, `Rainy = 2`, and `Stormy = 3`.
5. **Calculate descriptive statistics** — review measures such as count, mean, standard deviation, minimum, and maximum.
6. **Create visualizations** — produce five plots:
   - Temperature distribution
   - Average temperature and humidity by weather type
   - Humidity versus temperature
   - Weather type across pressure groups
   - Correlation heatmap of weather features
7. **Export data** — save the raw and cleaned datasets as Excel files.

## How to Run

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload `Weather_EDA_Colab.ipynb`, or open it from your Google Drive.
3. Run the notebook cells from top to bottom using **Runtime → Run all**.
4. When the notebook finishes, download `messy_weather_data.xlsx` and `cleaned_weather_data.xlsx` from the Colab file panel if needed.

### Use Your Own Dataset

The notebook includes an example for reading an Excel or CSV file. To use your own dataset, upload it to the Colab session and update the file name and column names in the notebook so they match your data.

## Data Cleaning Details

- Numeric missing values in `Temperature`, `Humidity`, `Wind_Speed`, and `Visibility` are replaced with their respective medians.
- Weather labels are encoded as:

  | Weather type | Code |
  |---|---:|
  | Sunny | 0 |
  | Cloudy | 1 |
  | Rainy | 2 |
  | Stormy | 3 |

## Visualizations

The notebook generates these plots to help explore the data:

| Plot | Purpose |
|---|---|
| Temperature distribution | Shows how temperature values are distributed. |
| Average temperature and humidity by weather type | Compares the average values across weather categories. |
| Humidity vs. temperature | Displays the relationship between humidity and temperature. |
| Weather type across pressure groups | Compares weather-category counts for low and normal/high pressure groups. |
| Correlation heatmap | Displays correlations between numerical weather features. |

## Results and Interpretation

Run the notebook to see the actual descriptive statistics and charts. Because the dataset is generated synthetically, any patterns found are for learning and demonstration only and should not be interpreted as real-world weather forecasts.

## GitHub Upload Guide

1. Create a GitHub account at [GitHub](https://github.com/).
2. Create a new repository, for example `weather-eda`.
3. Upload `README.md`, `Weather_EDA_Colab.ipynb`, and the `assets` folder.
4. Commit the changes.
5. Share the repository link with your teacher or classmates.

The image below is the supplied GitHub upload guide for reference.

![GitHub upload guide](assets/github-upload-guide.jpeg)

## Future Improvements

- Use a real weather dataset from a reliable source.
- Add more records and include date/time-based analysis.
- Investigate outliers and validate the cleaning choices.
- Add interactive charts or a dashboard.

## Author

Add your name, register number, department, and institution here before submitting the project.
