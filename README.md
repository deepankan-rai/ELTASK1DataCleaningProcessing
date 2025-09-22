# ELTASK1DataCleaningProcessing

Steps Performed :

1. Data Import & Exploration
Loaded the Titanic dataset using pandas.
Explored basic info (shape, data types, missing values, sample rows).

2. Handling Missing Values
Age → Filled with median (less affected by outliers).
Embarked → Filled with mode (most common port).
Cabin → Filled with "Missing" (preserves info instead of dropping).

3. Encoding Categorical Features
Converted Sex to numeric: male=1, female=0.
Converted Embarked using LabelEncoder.
Dropped Name and Ticket (not essential for basic ML models).

4. Feature Scaling
Standardized numerical columns (Age, Fare, SibSp, Parch) using StandardScaler
→ ensures mean=0, standard deviation=1 for ML algorithms.

5. Outlier Detection & Removal
Visualized outliers using boxplots.
Removed rows with extreme values using IQR method
→ keeps data clean and reduces noise.

6. Correlation Analysis
Plotted a correlation heatmap to understand relationships between features and Survived.

7. Final Cleaned Dataset
Saved processed dataset as Titanic-Cleaned.csv for use in ML models.
