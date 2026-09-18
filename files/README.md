# Category Intelligence — Retail Product Performance EDA

**Calibo AI Academy — Phase 1, Mini Use Case 01**

## Project Objective

This project analyzes six months (January–June 2026) of retail transaction data to give a Category
Manager an evidence-based view of product performance ahead of a quarterly supplier review. It answers
three questions:

1. Which categories and products are growing or declining, and by how much?
2. Which products deserve to be challenged in a supplier review?
3. Is the current discounting strategy generating a meaningful revenue return?

## Dataset

- **File:** `MUC01_Retail_Sales_Dataset.csv`
- **Coverage:** January 1, 2026 – June 30, 2026 (~107,836 transactions)
- **Categories:** Electronics, Apparel, Grocery, Home & Kitchen, Personal Care (5 products each, 25 total)
- **Columns:** `transaction_id`, `date`, `store_id`, `store_city`, `category`, `product_name`,
  `units_sold`, `unit_price`, `revenue`, `discount_pct`

The dataset is used as-is; no values were modified or fabricated.

## Tools Used

- Python 3
- pandas, NumPy — data loading and analysis
- matplotlib, seaborn — visualization
- Jupyter Notebook — analysis environment

## How to Install Requirements

From the project folder:

```bash
pip install -r requirements.txt
```

## How to Run the Notebook

1. Make sure `MUC01_Retail_Sales_Dataset.csv` is in the same folder as the notebook.
2. Launch Jupyter:
   ```bash
   jupyter notebook
   ```
3. Open `Varshitha_MUC01_KLU_Notebook.ipynb`.
4. Run all cells (**Kernel → Restart & Run All**). The notebook uses only a relative path
   (`pd.read_csv("MUC01_Retail_Sales_Dataset.csv")`) and does not depend on any external files or
   machine-specific paths.

## Expected Outputs

Running the notebook produces:

- Data quality checks (nulls, duplicates, types, summary statistics)
- A monthly revenue trend line chart across all five categories
- A top-2 / bottom-2 product summary table for every category
- A discount-bracket effectiveness bar chart (average revenue per transaction by discount level)
- Day-of-week and monthly revenue pattern charts
- A written Category Manager Briefing, Key Findings, and Limitations section, all grounded in the
  actual calculated numbers from the dataset

A companion Word document, `Varshitha_MUC01_KLU_Summary.docx`, summarizes the same findings for
individual submission.

## Project Files

```
MUC01_Retail_Sales_Dataset.csv        Source dataset
Varshitha_MUC01_KLU_Notebook.ipynb    Full EDA notebook
Varshitha_MUC01_KLU_Summary.docx      ~400-word executive summary
README.md                             This file
requirements.txt                      Python dependencies
```
