# Atidot Data Analyst - Home Assignment

## Setup Instructions

1. Place `policies.csv` in the same directory as the notebook
2. Open `analysis.ipynb` in Jupyter Notebook
3. Run all cells

**Requirements:** Python 3.8+, pandas, numpy, matplotlib, seaborn

## Summary of Findings

### Data Quality
Identified 3 issues: date columns as text (fixed), missing income_band ~9% (replaced with "Unknown"), unknown gender "U" ~4% (kept as-is).

### Key Insights

**1. Payment Frequency is the strongest churn predictor**
- Monthly: 15.5% churn vs Annual: 7.7% (2x difference)

**2. Acquisition Channel matters**
- Agent: lowest churn (12%) and largest volume (45%)
- Bank: highest churn (16%)

**3. Customer Tenure is critical**
- Churned customers have 25% shorter tenure on average

**4. Product Type influences retention**
- Term: lowest churn (12.1%), most cost-effective
- Universal/Whole: higher churn (14.5%)

### Recommendations
1. Incentivize Monthly → Annual payment conversion
2. Early engagement program for first 12-24 months
3. Review Bank channel onboarding process
4. Build predictive churn model using identified risk factors
