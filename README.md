# Task-1-Data-Cleaning-Preprocessing
Task 1: Data Cleaning &amp; Preprocessing
To clean and prepare the Titanic dataset for machine learning by handling missing data, encoding categories, scaling numerical values, and removing outliers.
 Explored the Dataset
-Loaded the Titanic dataset (Titanic-Dataset.csv) using pandas
Checked:
Data types (df.info())
Summary statistics (df.describe())
Null values (df.isnull().sum())
-Handled Missing Values  
Age column: Filled missing values using median
Cabin column: Filled with 'Unknown'
Embarked column: Dropped rows with missing values
-Encoded Categorical Variables
Used One-Hot Encoding (pd.get_dummies()) to convert:
Sex → into a numerical column
Embarked → into multiple columns (one per category)
-Standardized Numerical Features
Used StandardScaler() to scale:
Age
Fare
Result: These columns now have a mean of 0 and standard deviation of 1
-Visualized & Removed Outliers
Used Seaborn’s boxplot to spot outliers in the Age column
Applied IQR method to remove extreme outliers
