# MSDS-451-Week4-TermProject-CheckpointA

## 📘 Overview
This repository contains all materials for **Week 4 – Term Project Checkpoint A** of the *MSDS 451: Programming for Data Science* course.  
The project focuses on designing an **actively managed exchange-traded fund (ETF)** targeting large-cap technology companies — **Apple (AAPL)**, **Microsoft (MSFT)**, and **NVIDIA (NVDA)** — which are influenced by innovation cycles, monetary policy, and investor sentiment surrounding AI and cloud technologies.

The ETF is built around a **data-driven, rule-based framework** that combines traditional financial indicators with alternative data sources such as macroeconomic trends, sentiment, and public search interest.

---

## 📂 Repository Structure
```
│
├── 📄 README.md
├── 📄 requirements.txt
│
├── 📂 reports/
│ └── Week4_Term_Project_CheckpointA_Research_Report_ShrutiKalaskar.pdf
│
├── 📂 notebooks/
│ └── quick_eda.ipynb
│
├── 📂 week4_outputs/
│ ├── prices_levels.png
│ ├── prices_normalized.png
│ ├── daily_returns.png
│ ├── rolling_vol_21d.png
│ ├── correlation_matrix.png
│ ├── correlations.csv
│ └── metrics.csv
```
## How to Run the Notebook

### Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/MSDS451-Term-Project.git
cd MSDS451-Term-Project
```
### Install Dependencies

Use a Python 3.8+ environment and install required packages:
```
pip install -r requirements.txt
```
### Run the Notebook
```
jupyter notebook notebooks/quick_eda.ipynb
```
The notebook will:

Download adjusted close prices for AAPL, MSFT, and NVDA (2019–2024)

Compute daily returns, volatility, and Sharpe ratios

Generate plots and metrics saved under /week4_outputs/

### EDA Highlights
Metric	AAPL	MSFT	NVDA
Annualized Return	0.23	0.26	0.49
Annualized Volatility	0.21	0.22	0.36
Sharpe Ratio	1.00	1.09	1.31

- NVDA demonstrates the highest return and Sharpe ratio, reflecting its strong performance during the AI-driven cycle.
- Correlations between daily returns (≈0.65–0.85) indicate shared macro-tech exposure with limited but present diversification.
- Volatility analysis reveals identifiable risk regimes, notably during COVID-19 and 2022–2023 rate cycles.

### Key Outputs
File	Description
prices_levels.png	Adjusted close prices for AAPL, MSFT, and NVDA
prices_normalized.png	Normalized price index (100 = start of 2019)
daily_returns.png	Daily percentage returns across all stocks
rolling_vol_21d.png	21-day rolling volatility (annualized)
correlation_matrix.png	Heatmap of correlations among daily returns
metrics.csv	Annualized return, volatility, and Sharpe summary
correlations.csv	Pairwise correlation matrix values

### Research Report
Week 4 Term Project Checkpoint A – Research Report (PDF)

The report defines:

-  The investment philosophy behind the ETF
-  A literature review (Grinold & Kahn, Markowitz, Sharpe, Covel, etc.)
-  Data sources, methodology, and signal framework
-  Exploratory findings supported by EDA charts and metrics
-  Future roadmap toward a fully systematic, algorithmic ETF strategy

