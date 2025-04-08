# Multimodal-Financial-Time-Series-Forecasting-Sentiment-Analysis-and-LLM-Only-Approaches
This repository contains two Jupyter Notebooks for financial time series forecasting and robustness testing using Apple (AAPL) stock data: Multimodal_Financial_Time_Series_Forecasting.ipynb and Robustness_Testing_Financial_Forecasting.ipynb.

Project Overview
Multimodal_Financial_Time_Series_Forecasting.ipynb: Compares sentiment analysis and LLM-only approaches for forecasting AAPL stock prices (Apr 1, 2020 - Dec 31, 2024). Calculates technical indicators, fits traditional supervised learning models and deep learning models for the sentiment analysis aproach, and constructs prompts for the LLM-only approach.
Robustness_Testing_Financial_Forecasting.ipynb: Follow the same steps as in the Multimodal_Financial_Time_Series_Forecasting.ipynb. Tests robustness of forecasting approaches for AAPL stock prices (Jun 1, 2024 - Mar 10, 2025). Calculates technical indicators, predicts with the fine-tuned traditional supervised learning models and deep learning models in Multimodal_Financial_Time_Series_Forecasting.ipynb for the sentiment analysis aproach, and predicts with the fine-tuned LLM for the LLM-only approach.

Prerequisites
Python 3.12.4+
Jupyter Notebook/JupyterLab
Internet connection (for yfinance)

Python Libraries
Install required libraries:
pip install yfinance numpy pandas ta matplotlib seaborn

Files
Notebooks: Multimodal_Financial_Time_Series_Forecasting.ipynb, Robustness_Testing_Financial_Forecasting.ipynb
CSVs (place in same folder as notebooks): 

Setup Instructions
1. Clone/download the repository:
git clone <repository-url>
cd financial_forecasting
2. Set up a virtual environment (optional):
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
3. Install libraries:
pip install yfinance numpy pandas ta matplotlib seaborn
4. Launch Jupyter Notebook:
jupyter notebook
5. Verify CSVs are in the folder.

Running the Notebooks
Open each notebook in Jupyter and run cells sequentially.
Multimodal Notebook:
  Runtime: ~7463.91s (2+ hours).
Robustness Notebook:
  Runtime: ~35.89s.
  
Notes
Missing Data: Load CSVs for test_multimodal_data, test_close, and test_prompts_predictions before running relevant cells.
Internet Dependency: yfinance requires an internet connection.
Plot File Name: Robustness notebook saves plot as Actual_vs_Predicted_Closing_Prices_Google.png (misleading for AAPL data; consider renaming to Actual_vs_Predicted_Closing_Prices_AAPL.png).

Troubleshooting
Module Not Found: Ensure libraries are installed.
File Not Found: Verify CSVs are in the folder.
Internet Issues: Check connection for yfinance.
Plotting Errors: Ensure datasets are defined with required columns.

License
For educational/research purposes. Comply with yfinance terms.

Contact
Open an issue in the repository or contact the maintainer.
