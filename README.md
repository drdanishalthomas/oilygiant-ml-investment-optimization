# OilyGiant Oil Well Investment Optimization

## Project Overview
Machine learning project to identify the most profitable region for oil well development while minimizing financial risk. Built predictive models and bootstrap validation framework to support capital allocation decisions for 200 potential well locations across three geographic regions.

## Business Problem
OilyGiant needs to select the optimal region for developing 200 new oil wells from three candidate regions. With a budget of $100M ($500k per well) and profit target of $4.5M minimum per well, the goal is to maximize profit while minimizing risk of losses.

## Technical Approach

### Data Processing
- Analyzed 100,000 oil well measurements across three regions
- Features: f0, f1, f2 (geological survey parameters)
- Target: Volume of oil reserves (thousand barrels)

### Modeling
- **Algorithm:** Linear Regression (Scikit-learn)
- **Validation:** Bootstrap simulation with 1,000 iterations
- **Metrics:** RMSE for prediction accuracy, profit distribution analysis

### Risk Analysis
- Calculated profit distributions using bootstrap sampling
- Identified break-even thresholds (111.11 barrels minimum per well)
- Assessed probability of losses for each region

## Key Findings

| Region | Avg Predicted Reserves | RMSE | Expected Profit | Risk of Loss |
|--------|----------------------|------|----------------|--------------|
| Region 0 | 92.5 barrels | 37.6 | $3.32M | 6.2% |
| Region 1 | 68.7 barrels | 0.89 | **$7.04M** | **0%** |
| Region 2 | 95.0 barrels | 40.0 | $2.42M | 0.6% |

### Recommendation
**Invest in Region 1** - Highest expected profit ($7.04M) with zero risk of losses, despite lower average predicted reserves. Superior model performance (RMSE=0.89) provides confidence in predictions.

## Technologies Used
- **Python 3.x**
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib
- **Techniques:** Linear Regression, Bootstrap Validation, Statistical Analysis
- **Tools:** Jupyter Notebook

## Project Structure
```
├── notebook.ipynb          # Main analysis notebook
└── README.md              # Project documentation
```

## Skills Demonstrated
- Predictive modeling and regression analysis
- Bootstrap validation and statistical simulation
- Risk assessment and financial modeling
- Data-driven decision making for capital allocation
- Business-focused technical communication

## Author
Dr. Danisha L. Thomas  
[LinkedIn](https://www.linkedin.com/in/dr-danisha-l-thomas/) | [Portfolio](https://drdanishalthomas.github.io/my-portfolio/)
