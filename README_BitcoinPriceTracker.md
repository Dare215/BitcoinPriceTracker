# Bitcoin Price Tracker & EDA

**Author:** Darious Brown  
**GitHub:** [Dare215](https://github.com/Dare215)  
**Email:** dariousbrown3@icloud.com  

## 1) Project Overview
This project analyzes historical Bitcoin trading data to investigate the relationship between **daily price changes**, **trading volume**, and **market capitalization**.  
**Hypothesis:** Bitcoin's daily price change is significantly influenced by its trading volume and market capitalization, with higher volumes and larger market caps correlating to more stable price movements.

## 2) Dataset
- **Training Data:** `bitcoin_price_Training - Training.csv`  
- **Test Data:** `bitcoin_price_1week_Test - Test.csv`  
- Columns: `Date`, `Open`, `High`, `Low`, `Close`, `Volume`, `Market Cap`
- **Data Source:** Kaggle (Bitcoin historical prices dataset)

## 3) Key Features
- **Descriptive Statistics:** Histograms, PMF, and normal distribution fits for daily price changes
- **Correlation Analysis:** Pearson correlation between Volume & Market Cap (0.89), High & Low (1.00)
- **Scatterplots:**  
  - Volume vs. Daily Price Change  
  - Volume vs. Market Cap  
  - High vs. Low
- **Covariance Analysis**
- **Insights:** Extreme buying/selling pressure on certain days, strong correlation between market cap and volume.

## 4) Project Structure
```
bitcoin-price-tracker/
│── BitcoinTracker.ipynb       # Main analysis notebook
│── bitcoin_price_Training.csv # Training dataset
│── bitcoin_price_1week_Test.csv # Test dataset
│── images/                    # Exported charts and visuals
│── README.md
│── requirements.txt
```

## 5) How to Run

### Option A — Python / Terminal
```bash
# Create and activate a virtual environment
python -m venv .venv
source .venv/bin/activate   # Mac/Linux
.venv\Scripts\activate      # Windows

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook BitcoinTracker.ipynb
```

### Option B — PyCharm
1. Open the folder in PyCharm  
2. Configure a Python interpreter (point to `.venv`)  
3. Install requirements from `requirements.txt`  
4. Run the notebook inside PyCharm's Jupyter integration

### Option C — GitHub Desktop
1. Add the local repository to GitHub Desktop  
2. Commit all files (including `README.md` and `requirements.txt`)  
3. Push to a public GitHub repository  
4. The README will be displayed automatically

## 6) Results Summary
- **Volume vs. Market Cap:** Strong positive correlation (0.89)
- **High vs. Low:** Perfect correlation (1.00)
- **Daily Price Change Distribution:** Heavy tails, indicating days with extreme volatility.
- **Fit Parameters:** μ = 1.46, σ = 36.52

## 7) Ethical Considerations
- Financial models should include risk disclaimers  
- Cryptocurrency investments are highly volatile and speculative  
- Avoid using models for financial advice without appropriate licensing  

## 8) Future Research
- Incorporate **news sentiment analysis** from social media and global events
- Explore non-linear models (Random Forest, LSTMs)
- Evaluate regulatory and political impacts

## 9) License
MIT License — Free to use with attribution.
