# 📊 Regression Modeling: Diabetes & Medical Cost Personal Datasets

This project explores predictive modeling using two healthcare-related datasets:

- **Diabetes Dataset** (from `sklearn.datasets`)
- **Medical Cost Personal Dataset** ([Kaggle](https://www.kaggle.com/datasets/mirichoi0218/insurance))

The goal is to benchmark regression strategies across datasets with different feature relationships, using techniques such as:

- Polynomial feature expansion  
- Feature engineering  
- Hyperparameter tuning  
- Ensemble modeling (VotingRegressor, RandomForest, XGBoost)  
- Cross-validation and R² performance tracking

---

## ⚙️ Environment Setup

To run this project locally, follow these steps:

```bash
# Clone the repository
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

# Create and activate a conda environment
conda create -n regression-env python=3.10
conda activate regression-env

# Install required libraries
conda install pandas numpy matplotlib seaborn scikit-learn
pip install xgboost

# Launch Jupyter Notebook
jupyter notebook
```

## 🧪 Requirements
The project uses the following Python libraries:

pandas

numpy

matplotlib

seaborn

scikit-learn

xgboost

These can be installed via conda and pip as shown above.

## 📁 Project Structure
notebooks/ — Jupyter notebooks with full model search workflows

data/ — Raw and processed datasets (if applicable)

requirements.txt — Python dependencies

README.md — Project overview and setup instructions

## 📌 Key Insights
The Diabetes dataset showed weak feature-target relationships, with R² scores rarely exceeding 0.60.

The Medical Cost dataset revealed strong dependency on smoking status, enabling R² scores above 0.87.

Feature engineering (e.g., smoker-based multipliers) improved performance by approximately 0.02 R².

Using random_state=0 consistently yielded better reproducibility and model performance.

Final VotingRegressor configuration achieved R² > 0.90 on the test set with cross-validation R² ≈ 0.85.

📬 Contact
For questions or collaboration, feel free to reach out via GitHub Issues or connect on LinkedIn.
