Getting Started
Prerequisites

    Python 3.9 or higher
    pip

Step 1 — Clone the repository

Bash

git clone https://github.com/your-username/heart-disease-prediction.git
cd heart-disease-prediction

Step 2 — Create a virtual environment

Bash

# Linux / macOS
python3 -m venv venv
source venv/bin/activate

# Windows
python -m venv venv
venv\Scripts\activate

Step 3 — Install dependencies

Bash

pip install -r requirements.txt

Step 4 — Generate data and train models

Bash

python data/generate_data.py
python notebooks/heart_disease_analysis.py

Step 5 — Launch the Streamlit application

Bash

streamlit run app/app.py

Open your browser at : http://localhost:8501
Streamlit Application Pages
Page	Content
Home and Prediction	Input form + probability gauge + diagnosis card
Data Analysis	Dataset overview, distributions, boxplots, correlation matrix
Model Performance	Comparison table, ROC curves, feature importance chart
About	Pipeline description, features, metrics, disclaimer
Tech Stack
Category	Libraries
Data manipulation	pandas, numpy
Visualization	matplotlib, seaborn, plotly
Machine Learning	scikit-learn, xgboost
Model saving	joblib
Web application	streamlit
Visualizations Generated
Figure	Description
01	Target variable distribution (bar + pie chart)
02	Numeric feature distributions by class
03	Correlation heatmap
04	Boxplots by class
05	Categorical features vs target
06	Model comparison + ROC curves
07	Confusion matrix (best model)
08	Feature importance (Random Forest)
09	Precision-Recall curves
Possible Improvements

    Apply SMOTE to handle class imbalance
    Add SHAP values for individual prediction explainability
    Use the real UCI Cleveland dataset
    Expose the model through a REST API with FastAPI
    Deploy the app on Streamlit Cloud or Heroku
    Add model logging and monitoring

