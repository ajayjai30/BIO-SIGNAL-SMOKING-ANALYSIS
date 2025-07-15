# Biosignal Analysis for Smoking

## Project Overview
This project analyzes biosignal data to predict smoking status using data science and machine learning techniques. The analysis includes data preprocessing, exploratory data analysis (EDA), feature selection, and training multiple classification models to identify smokers based on biosignal and demographic features.

## Tech Stack
- **Python**: Programming language used for the entire analysis.
- **Pandas**: Data manipulation and analysis.
- **NumPy**: Numerical computing.
- **Seaborn**: Statistical data visualization.
- **Matplotlib**: Plotting and visualization.
- **Scikit-learn**: Machine learning library used for feature selection, model training, and evaluation.

## Dataset
The dataset contains biosignal measurements and demographic information related to smoking status. Key features include age, gender, tartar presence, and various biosignal indicators. The target variable is `smoking`, indicating whether the individual is a smoker.

## Data Preprocessing
- Dropped irrelevant columns such as `oral` and `ID`.
- Encoded categorical variables manually (e.g., gender: M/F to 0/1, tartar: Y/N to 1/0).
- Checked for missing values and data types.
- Standardized numerical features before model training.

## Exploratory Data Analysis (EDA)
- Visualized distributions of numerical features using boxplots.
- Analyzed categorical variables with bar plots and count plots.
- Examined the proportion of smokers using pie charts.
- Investigated age distribution among smokers with histograms.
- Found that most smokers are male and the highest smoking prevalence is around age 40.

## Feature Selection
- Used `ExtraTreesClassifier` to identify the most important features influencing smoking status.
- Selected top features based on importance scores for model training.

## Machine Learning Models
- **Logistic Regression**: Baseline linear model for classification.
- **Decision Tree Classifier**: Tree-based model for classification.
- **Bagging Classifier**: Ensemble method using multiple decision trees.
- **Extra Trees Classifier**: Ensemble of randomized decision trees.
- **Random Forest Classifier**: Ensemble of decision trees with bootstrap aggregation.

Each model was trained on the selected features and evaluated using classification reports and accuracy scores.

## How to Run
1. Ensure Python 3.6+ is installed.
2. Install required libraries:
   ```
   pip install pandas numpy seaborn matplotlib scikit-learn
   ```
3. Place the dataset CSV file (`smoking.csv`) in the appropriate path or update the script to point to the dataset location.
4. Run the script:
   ```
   python biosignal_analysis_for_smoking.py
   ```

## License
This project is open source and available for use and modification.
