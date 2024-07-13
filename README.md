# ML Project with XGBoost | Car Insurance Claims Prediction

## ➤ Basic Data Cleaning and Column Renaming
▶Initial basic data cleaning involves identifying missing values and ensuring data integrity without splitting into training and testing sets.
▶To enhance clarity, columns are renamed for better descriptive accuracy, facilitating easier data interpretation.

## ➤Handling Currency Symbols and Prefixes
▶Currency symbols and prefixes are removed to standardize numerical data for proper analysis without distortions.
▶Functions are defined and applied to eliminate these elements from the dataset in preparation for further processing.

## ➤Creating Train and Test Splits with Stratified Sampling
▶Stratified sampling, based on the claim value feature, ensures unbiased representation in the test set.
▶Bins are created to categorize data for coherent division into training and testing subsets, improving model accuracy and fairness.

## ➤Exploring Correlations through Data Analysis
▶The exploration of correlations involves joining predictor and target variables to assess relationships within the dataset.
▶Modifications are suggested for categorical data handling to enhance correlation analysis and derive meaningful insights for the model building process.

## ➤Feature Mapping and Data Exploration
▶The mapping of binary values is demonstrated by assigning specific values such as 1 or 0 to different categories like gender.
▶The next step involves applying this mapping to update the features by iterating through each binary column.
▶By creating a correlation matrix and utilizing a heatmap, the correlations between various features and the target variable (claim status) can be visually assessed.

## ➤Data Imputation and Encoding
▶After identifying unnecessary features like "red vehicle" due to lack of correlation, the focus shifts to handling missing values.
▶Imputation begins by employing a K Nearest Neighbors (KNN) imputer for numerical features and a simple imputer for categorical features.
▶Categorical features are encoded using various techniques like one-hot encoding for non-ordinal features and ordinal encoding for features with a specific order.

## ➤Feature Engineering and Model Selection
▶Knowing all values for one of the one-hot encoded features allows perfect prediction of the remaining, indicating perfect multicollinearity.
▶The Variance Inflation Factor (VIF) can identify multicollinearity by checking each feature's VIF.
▶Dropped dummy variables to avoid the dummy variable trap, ensuring VIF values are below five, which is acceptable.
▶Tested various models using cross-validation to prevent overfitting and evaluate performance.
▶Box plot visualization highlighted best and worst performing models; XGBoost was chosen for its effectiveness.
▶Tuned hyperparameters of XGBoost due to its efficiency for this task.
Data Pre-processing and Pipeline Verification
