Commodity–FX Predictive Modeling (Python)

Analyzing how major commodities influence currency movements.

📌 Overview

This project analyzes the relationship between key commodities and major FX pairs using a quantitative and data-driven approach. The study evaluates whether changes in oil, copper, and gold prices can explain or predict movements in currencies such as NOK, CAD, EUR/USD, CLP, COP, and RUB.

The entire analysis is contained in the notebook MLDivisas-Commodities.ipynb, where different machine learning models are compared using time-series cross-validation.

📂 Repository Contents
MLDivisas-Commodities.ipynb             # Full analysis, preprocessing, ML models, and plots
/data/                 # Folder containing the dataset (user-provided)
README.md


⚠️ To run the notebook, you only need to update the dataset file path inside MLDivisas-Commodities.ipynb.

🔍 Commodity–FX Pairs Analyzed
Commodity	Currency Pair
Oil	NOK, CAD, RUB
Copper	CLP, COP
Gold	EUR/USD
🧠 Methodology Summary
1. Data Processing

Import raw historical prices

Merge and align time series

Compute daily returns

Train/test split with TimeSeriesSplit

2. Machine Learning Models

Linear Regression

Ridge (L2)

Lasso (L1)

Random Forest

Gradient Boosting

Support Vector Regression (RBF)

3. Evaluation

R² with time-series CV

Error metrics (MAE, RMSE)

Best model selected for each commodity–FX pair

⭐ Key Findings
Commodity → FX	Predictability	Best Model
Oil → RUB	Very Low	Lasso
Oil → NOK	Medium	Linear / Ridge
Oil → CAD	Medium	Lasso
Gold → EUR/USD	High	Linear / Ridge
Copper → CLP	High	Linear / Ridge
Copper → COP	Medium	Linear / Ridge
📈 How to Run the Project
1. Clone the repo
git clone https://github.com/yourusername/Commodity-FX-Modeling.git
cd Commodity-FX-Modeling

2. Install dependencies

(You can adapt this list based on your environment.)

pip install pandas numpy scikit-learn matplotlib seaborn

3. Update dataset path

Inside MLDivisas-Commodities.ipynb, modify the line where the data is loaded:

df = pd.read_csv("YOUR/DATA/PATH.csv")

4. Run the notebook

Open and execute:

MLDivisas-Commodities.ipynb

👥 Authors

Hugo Cortazar

Gonzalo Casado

