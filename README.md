# HeartDisease_analysis
Analysis of dataset on Heart disease on different parameters like age, gender, cholestrol level, blood pressure, heart rate. 

## Understanding Key Risk Indicators
Heart disease is one of the leading causes of death worldwide. Identifying risk factors and understanding their impact can help develop strategies for early detection and prevention. This project aims to analyze a dataset of heart disease patients to explore patterns and correlations among key health indicators, such as cholesterol levels, blood pressure, and age, to determine their relationship with heart disease.

## Dataset
[Heart Disease Data](https://www.kaggle.com/datasets/redwankarimsony/heart-disease-data)
This dataset contains 303 records with 14 attributes, including patient demographics, medical test results, and a target variable indicating the presence of heart disease.

## Features
1. **Exploratory Data Analysis (EDA):**
   - General information about the dataset:
     - **Number of rows:** 920
     - **Number of columns:** 16
     - **Missing values:**
       - `trestbps`: 59
       - `chol`: 30
       - `fbs`: 90
       - `restecg`: 2
       - `thalch`: 55
       - `exang`: 55
       - `oldpeak`: 62
       - `slope`: 309
       - `ca`: 611
       - `thal`: 486
   - Distribution of target variables (`num`):
     - 0 (No heart disease): 411 patients
     - 1: 265 patients
     - 2: 109 patients
     - 3: 107 patients
     - 4: 28 patients
   - Gender distribution:
     - Male: 682 patients
     - Female: 238 patients
   - Age range of patients: 28 to 77 years

2. **Health Metrics Analysis:**
   - Average and median values for key metrics:
     - Resting blood pressure (`trestbps`):
       - Average: 132.13 mm Hg
       - Median: 130 mm Hg
     - Serum cholesterol (`chol`):
       - Average: 246.69 mg/dl
       - Median: 243 mg/dl
     - Maximum heart rate (`thalach`):
       - Average: 149.60 bpm
       - Median: 153 bpm
   - Outlier detection using Interquartile Range (IQR):
     - Outliers identified in both `chol` and `trestbps`.

3. **Visualizations:**
   - Age distribution histogram.
   - Comparison of average cholesterol levels between patients with and without heart disease:
     - Average cholesterol (With Heart Disease): 263.66 mg/dl
     - Average cholesterol (Without Heart Disease): 223.47 mg/dl
   - Boxplots to visualize outliers for cholesterol and resting blood pressure.

4. **Insights:**
   - Patients with heart disease tend to have higher average cholesterol levels.
   - Significant outliers in cholesterol and resting blood pressure suggest further preprocessing might be needed for predictive modeling.
   - Exercise-induced angina (`exang`):
     - Patients with angina: 204
     - Patients without angina: 204
   - Counts of different chest pain types (`cp`):
     - Type 0: 496
     - Type 1: 204
     - Type 2: 90
     - Type 3: 130

## Setup and Requirements
### Prerequisites
- Python 3.7+
- Libraries:
  - pandas
  - matplotlib
  - seaborn

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Aiengineer360/HeartDisease_analysis.git
   cd HeartDisease_analysis
   ```
2. Install required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the dataset from Kaggle and place it in the project directory.

## Usage
1. Run the script to perform analysis:
   ```bash
   python analysis.py
   ```

2. Visualizations and statistical summaries will be displayed and saved in the output folder.

## Key Findings
- The dataset provides valuable insights into the relationship between health metrics and heart disease.
- Patients with heart disease tend to have higher average cholesterol levels compared to those without heart disease.
- Significant outliers were detected in cholesterol and resting blood pressure metrics, suggesting the need for further preprocessing in predictive modeling tasks.

## Contributing
Contributions are welcome! If you'd like to contribute, please fork the repository and submit a pull request with your improvements.

## Acknowledgments
- The dataset was sourced from [Kaggle](https://www.kaggle.com/datasets/redwankarimsony/heart-disease-data).
- Special thanks to the open-source community for the tools used in this project.

