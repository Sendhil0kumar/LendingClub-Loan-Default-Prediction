LendingClub Loan Default Prediction
Project Overview
This project focuses on building a machine learning model to predict the probability of loan default using historical data from the LendingClub platform. The primary objective is to develop a reliable credit risk model that can help identify potentially risky borrowers at the time of loan application, thereby protecting investor capital.

The analysis involved a comprehensive data preprocessing pipeline, exploratory data analysis, and the development and evaluation of several classification models, with a key focus on addressing the severe class imbalance present in the dataset.

Key Findings
Class Imbalance: The dataset is highly imbalanced, with only ~12% of loans resulting in a default ("Charged Off"). This was the primary challenge for the modeling process.

Model Performance: While baseline models failed, models that accounted for class imbalance (using techniques like class_weight='balanced' or SMOTE) were successful in identifying defaults.

Strategic Trade-Off: The final models present a strategic choice:

Logistic Regression (Balanced): Maximizes detection (59% Recall) at the cost of lower precision.

Tuned Random Forest: Offers higher precision (26%) but finds fewer defaults.

Top Predictors of Default: The most influential factors increasing default risk were found to be higher monthly installments and higher interest rates. Conversely, higher annual income and larger funded loan amounts were associated with a lower risk.

How to Use This Repository
Clone the repository:

git clone [https://github.com/your-username/lendingclub-project.git](https://github.com/your-username/lendingclub-project.git)


Download the Dataset:

The dataset is too large for GitHub. Please download it from the following link and place it in the project folder:

Download Dataset Here

Install the required libraries:

pip install -r requirements.txt


Run the analysis:

Open the loan_default_analysis.ipynb notebook in a Jupyter environment (like Jupyter Notebook, JupyterLab, or Google Colab).

Execute the cells in the notebook to see the full analysis from data cleaning to model evaluation.

File Structure
loan_default_analysis.ipynb: The main Jupyter notebook containing all the code and analysis.

README.md: This file.

requirements.txt: A list of necessary Python packages.

.gitignore: Specifies files for Git to ignore.
