# ARTI308-Lab6

# Heart Disease Classification

## Dataset

* File: `heart.csv`
* Rows: 1025 (original)
* Features: 14

## Data Cleaning Steps

### 1. Data Exploration

* Checked structure using `.info()` and `.describe()`
* Verified all columns are numeric
* Identified `target` as the label (0 = no disease, 1 = disease)

### 2. Missing Values

* No missing values found in the dataset

### 3. Duplicate Removal

* Found duplicate rows
* Removed duplicates
* Dataset reduced to 302 rows

### 4. Outlier Detection

* Used IQR method to detect outliers
* Removed extreme values
* Dataset reduced further after outlier removal

### 5. Data Consistency

* No negative or invalid values found
* All features are within logical ranges

### 6. Feature Engineering

* Created a new column `age_group` to categorize ages:

  * Young
  * Middle
  * Senior
  * Old

## Exploratory Data Analysis (EDA)

* Visualized target distribution using count plots
* Used heatmap to analyze feature correlations
* Used pairplot to observe relationships between variables


## Model Building

### 1. Feature Selection

* Input features: All columns except `target`
* Target variable: `target`

### 2. Train-Test Split

* Split dataset into training (70%) and testing (30%)

### 3. Model Used

* Logistic Regression

### 4. Training

* Trained model using training dataset


## Model Evaluation

* Evaluated model using:

  * Accuracy Score
  * Confusion Matrix
  * Classification Report

* Model performance indicates good ability to classify heart disease cases


## Tools & Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn


