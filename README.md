# SOC-2025
#  Equity Research and Automation Using Python

This project automates equity research by combining stock data collection, technical analysis, visualization, and PDF report generation using Python. It focuses on analyzing Indian tech stocks such as **TCS**.

---

##  Final Deliverable

A single command generates a full stock analysis PDF with:
- ✅ Technical indicators (SMA, EMA)
- ✅ Volatility, skewness, kurtosis
- ✅ Chart image of price trends
- ✅ Automatically saved and organized report

---

##  What I Did (In Order)

###  Step 1: Set Up the Environment
- Installed Python and pip
- Created a virtual environment 
- Installed required packages:
  ```bash
  pip install -r requirements.txt

### ✅ Step 2: Built Core Modules

I created four Python modules inside the `src/` folder to modularize the workflow:

- **`data_fetcher.py`**  
  Uses `yfinance` to fetch historical stock data for a given ticker symbol.

- **`analyzer.py`**  
  Adds technical indicators like:
  - Simple Moving Average (SMA)
  - Exponential Moving Average (EMA)  
  And computes key statistics:
  - 📉 Volatility  
  - 📈 Skewness  
  - 📊 Kurtosis

- **`visualizer.py`**  
  Generates a stock price chart using `matplotlib`, overlays SMA/EMA lines, and saves the image as a `.png` file.

- **`reporter.py`**  
  Creates a clean, professional PDF report using the `fpdf` library, which includes:
  - Statistical summary (volatility, skewness, kurtosis)
  - A full-size chart of the stock's performance

---

### ✅ Step 3: Connected Everything in `main.py`

I built a master script `main.py` to execute the full analysis pipeline:

- Fetch stock data from Yahoo Finance
- Calculate technical and statistical indicators
- Generate and save the stock chart
- Compile all results into a formatted PDF report



