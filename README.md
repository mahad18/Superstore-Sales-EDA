# Superstore Sales — Exploratory Data Analysis

An end-to-end EDA on 4 years (2014–2017) of retail transaction data from a US-based superstore, focused on uncovering what's actually driving sales and profit — and where the business is quietly losing money.

## Key Findings

- **Discounting is the single biggest profitability issue.** Orders with no discount average $67 profit; once discount crosses 20%, the average order flips to a $110 **loss**.
- **Furniture generates revenue but barely any profit** — similar sales to Technology, but only a 2.5% margin vs. Technology's 17%, driven almost entirely by heavy discounting.
- **Tables and Bookcases are actively losing money** despite strong sales volume ($207K in sales, -$17.7K profit for Tables).
- **Texas, Ohio, Pennsylvania, and Illinois** underperform — not from low demand, but from disproportionately heavy discounting.
- **Q4 is the strongest quarter every year**, driven by holiday and year-end corporate spending; Q1 is consistently the weakest. Sales grew 51% from 2014 to 2017.
- **Shipping speed has no meaningful effect on profit** — discount level is a far stronger driver.
- Customer segmentation surfaced an **"At Risk"** group: previously frequent buyers who've gone quiet — a clear target for re-engagement.

## Notebook Structure

1. The Data — load, clean, validate
2. Sales and Profit Overview — distributions, outliers
3. Categories and Products — margin analysis by category/sub-category
4. Regional and State Performance
5. Customer Segments
6. Discount Analysis — the core finding of the project
7. Time Trends and Seasonality
8. Shipping Analysis
9. Customer Loyalty Segmentation
10. Summary, Recommendations, and Conclusion

## Tools

- Python (pandas, numpy)
- matplotlib, seaborn for visualization
- Jupyter Notebook

## How to Run

```bash
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook Superstore_Sales_EDA_notebook.ipynb
```

The dataset (`superstore.csv`) is included in this repo — the notebook reads it directly from the same folder.

## Recommendations (from the notebook)

| Priority | Problem | Finding | Suggested Action |
|---|---|---|---|
| High | Heavy discounts causing losses | Orders above 20% discount average a $110 loss | Cap discounts at 20%; anything above needs approval |
| High | Tables and Bookcases losing money | Negative margins despite strong sales | Review pricing/discount policy for these sub-categories |
| Medium | Certain states underperforming | High discounting, not low demand, is the driver | Tighten discount approval in Central region states |
| Medium | At-risk customers | Frequent past buyers have gone quiet | Targeted re-engagement campaign |

## Author

Independent data analysis project exploring retail sales performance and profitability drivers.
