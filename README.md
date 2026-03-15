# ML4E-Task-1
YC Housing Price Prediction - Linear Regression from Scratch
ML4E Club Induction Task | NIT Rourkela
What this is
Predicting property sale prices using linear regression implemented from scratch in pure NumPy. No scikit-learn model was used anywhere in this project.

Dataset
NYC housing records. Features used: building_age, landuse, borough_x, block. Target: sale_price.

Preprocessing steps
Removed duplicate rows
Filled missing values with column median
Removed outliers using IQR method
Standardized features using z-score normalization (no sklearn, done manually)


Models
MYLR
Simple linear regression that takes a single feature. Uses the Ordinary Least Squares closed-form formula to find the exact slope and intercept in one pass with no iteration. Built to understand the math before extending to multiple features.
MYLR_Multiple
Multiple linear regression that takes all four features. Uses Gradient Descent to iteratively update one weight per feature and a bias term over 1000 epochs, minimising Mean Squared Error. This is the model used for final predictions.
              MYLR              MYLR_Multiple
Features      Single only       Any number
Method        OLS formula       Gradient Descent
Iterations    None              1000 epochs
Used here     No                Yes

How to run?
Place nyc_housing.csv in the same folder as the notebook
Open Housing_Regression_ML4E.ipynb in Jupyter
Run all cells from top to bottom


Libraries used
pandas, numpy, matplotlib — nothing else.

Files
Housing_Regression_ML4E.ipynb         main notebook with all code
nyc_housing.csv                       dataset
Housing_Regression_Explanation.docx   explanation of each step
README.md                             this file
