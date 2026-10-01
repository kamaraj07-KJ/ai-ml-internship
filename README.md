# AI & ML Internship – Task 1

## Data Cleaning & Preprocessing

This project was completed as part of an **AI & ML Internship – Task 1: Data Cleaning & Preprocessing**.

The objective of this task is to clean and prepare a raw dataset for further machine learning analysis.

## Dataset

**Dataset:** Titanic Dataset

The original dataset contains:

- **891 records**
- **10 columns**

The dataset contains information about passengers, including age, passenger class, gender, number of siblings/spouses, parents/children, fare, and survival status.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- Jupyter Notebook

## Data Preprocessing Steps

### 1. Data Loading and Exploration

The Titanic dataset was loaded using Pandas and explored to understand:

- Dataset shape
- Data types
- Missing values
- Duplicate records
- Basic statistical information

### 2. Data Cleaning

Missing values were identified and handled.

The missing values in the `Age` column were replaced using **median imputation**.

Unnecessary columns were removed:

- `PassengerId`
- `Name`
- `Ticket`

### 3. Categorical Encoding

Categorical features were converted into numerical form using **one-hot encoding**.

The following features were encoded:

- `Sex`
- `Pclass`

The resulting encoded features include:

- `Sex_male`
- `Pclass_2`
- `Pclass_3`

### 4. Feature Scaling

Standardization was applied to the numerical features:

- `Age`
- `SibSp`
- `Parch`
- `Fare`

`StandardScaler` from Scikit-learn was used to transform the numerical features to a common scale.

### 5. Outlier Detection and Removal

Outliers were visualized using **boxplots**.

The **Interquartile Range (IQR)** method was used to identify and remove outliers from the numerical features.

The dataset was reduced from:

**891 records → 561 records**

### 6. Final Dataset

After preprocessing, the final dataset contains:

- **561 records**
- **8 processed columns**

The processed dataset is ready for further machine learning analysis and model development.

## Key Insights

- Missing values in the `Age` column were successfully handled using median imputation.
- Unnecessary columns were removed to simplify the dataset.
- Categorical variables were converted into numerical features using one-hot encoding.
- Numerical features were standardized using `StandardScaler`.
- Boxplots and the IQR method were used for outlier detection.
- Outlier removal reduced the dataset from 891 to 561 records.
- The final dataset contains 561 records and 8 processed columns.

## Project Structure

```text
AI-ML-Internship-Task-1/
│
├── titanic_dataset.ipynb
├── titanic.csv
└── README.md
```

## Conclusion

The Titanic dataset was successfully cleaned and preprocessed by handling missing values, removing unnecessary columns, encoding categorical features, standardizing numerical features, and detecting and removing outliers using the IQR method.

The final processed dataset contains **561 records and 8 columns** and is suitable for further machine learning analysis and model development.

## Author

**Kamaraj T.**

B.Tech – Computer Science Engineering  
Data Science / AI-ML Fresher
