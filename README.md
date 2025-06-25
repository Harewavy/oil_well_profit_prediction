# Oil Well Profit Prediction

This machine learning project helps **OilyGiant**, a mining company, determine the most profitable region to develop a new oil well.  
By using linear regression and risk analysis with **bootstrapping**, the goal is to identify the region with the highest expected profit and acceptable risk level.

---

## Datasets

- `geo_data_0.csv`
- `geo_data_1.csv`
- `geo_data_2.csv`

### Features:
- `id` — unique oil well identifier
- `f0`, `f1`, `f2` — extracted geological features
- `product` — target variable: volume of reserves (in thousand barrels)

---

## Tools & Libraries

- Python
- pandas, numpy
- scikit-learn
- LinearRegression
- Bootstrapping (via NumPy)

---

## Project Workflow

1. Loaded and explored data from three regions
2. Trained a linear regression model for each region
3. Predicted oil reserve volumes and calculated RMSE
4. Selected top 200 wells from 500 explored per region
5. Calculated potential profit under business constraints
6. Applied **bootstrapping** (1000 samples) to simulate profit variability
7. Evaluated:
   - Mean profit
   - 95% confidence interval
   - Risk of loss (as probability)

---

## Business Constraints

- 200 wells selected for development
- Development budget: $100 million
- Revenue per 1,000 barrels: $4.5k
- Must choose a region with **risk of loss < 2.5%**
- From those, choose the region with the **highest average profit**

---

## Key Findings

- One region had a strong balance of high profit and low risk.
- Bootstrapping confirmed the expected profit and loss boundaries.
- Final region selection is justified using both statistics and business logic.

---

## How to Run

1. Clone this repository
2. Ensure all `geo_data_*.csv` files are in the same directory as the notebook
3. Open the notebook in Jupyter
4. Run all cells to reproduce the analysis and simulation

---

## Links

- [My LinkedIn](https://www.linkedin.com/in/ozturkkenes)
- [My GitHub](https://github.com/Harewavy)
