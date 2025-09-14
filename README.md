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

## Environment Setup

### Prerequisites
- Python 3.8 or higher
- pip package manager

### Installation

1. **Clone the repository:**
```bash
git clone https://github.com/Krishnanand-G/mmm_modelling_assessment.git
cd mmm_modelling_assessment
```

2. **Create virtual environment (recommended):**
```bash
python -m venv mmm_env
# Windows:
mmm_env\Scripts\activate
# macOS/Linux:
source mmm_env/bin/activate
```

3. **Install required packages:**
```bash
pip install pandas numpy matplotlib scikit-learn xgboost jupyter
```

### Running the Model

1. **Start Jupyter Notebook:**
```bash
jupyter notebook
```

2. **Open and run the model:**
   - Open `mmm_model.ipynb`
   - Run all cells (Cell → Run All)
   - Results will be saved to `mmmdataset_predicted.csv`

### Alternative: Run without Jupyter
```bash
python -c "import jupyter; jupyter nbconvert --to python mmm_model.ipynb; python mmm_model.py"
```

## Data

104 weeks of marketing data including:
- Facebook, Google, TikTok, Instagram, Snapchat spend
- Email/SMS sends
- Social followers
- Revenue

Author: Krishnanand-G
