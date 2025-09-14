# MMM Modeling Project

Marketing Mix Modeling using XGBoost to predict revenue from marketing spend.

## What it does

- Predicts Google ad spend from other marketing channels
- Predicts revenue from all marketing activities
- Uses 104 weeks of data (Sept 2023 - Sept 2025)

## Files

- `Assessment 2 - MMM Weekly.csv` - Raw data
- `mmm_model.ipynb` - Jupyter notebook with the model
- `mmmdataset_predicted.csv` - Results with predictions

## Model Performance

**Stage 1 (Google Spend):**
- R² = 0.943
- RMSE = $441

**Stage 2 (Revenue):**
- R² = 0.944  
- RMSE = $22,054

## Key Findings

- SMS sends are the biggest predictor of revenue (38% importance)
- Social followers matter a lot (31% importance)
- Google spend can be predicted from other channels
- Total ROI is 5.71x

## How to run

1. **Clone the repository:**
```bash
git clone https://github.com/Krishnanand-G/mmm_modelling_assessment.git
cd mmm_modelling_assessment
```

2. **Install prerequisites:**
```bash
pip install pandas numpy matplotlib scikit-learn xgboost jupyter
```

3. **Run the notebook:**
```bash
jupyter notebook mmm_model.ipynb
```

## Data

104 weeks of marketing data including:
- Facebook, Google, TikTok, Instagram, Snapchat spend
- Email/SMS sends
- Social followers
- Revenue

Author: Krishnanand-G
