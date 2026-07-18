# Rossmann Store Sales Forecasting

Sales forecasting project on the [Rossmann Store Sales](https://www.kaggle.com/c/rossmann-store-sales) Kaggle dataset. Predicts daily sales for 1,000+ Rossmann drug stores using historical sales, promotions, holidays, and store attributes.

---

## Overview

- Cleaned and preprocessed historical sales data — handled missing values, encoded categorical features (`StateHoliday`, `SchoolHoliday`)
- Engineered time-based features (Year, Month) from the `Date` column
- Performed exploratory data analysis — correlation heatmaps, distribution checks — to identify key sales drivers
- Trained and compared multiple regression models to forecast daily sales
- Evaluated models using RMSE and R² score

## Results

| Model | R² Score | RMSE |
|---|---|---|
| Linear Regression | 0.548 | 2567.85 |
| Decision Tree Regressor | 0.903 | — |
| **Random Forest Regressor** | **0.931** | — |

**Random Forest performed best** on the held-out test split.

## Visuals

<p align="center">
  <img src="outputs/Screenshot 2026-07-18 214033.png" width="600"><br>
  <img src="outputs/Screenshot 2026-07-18 214101.png" width="600"><br>
  <img src="outputs/Screenshot 2026-07-18 214121.png" width="600"><br>
  <img src="outputs/Screenshot 2026-07-18 214143.png" width="600"><br>
  <img src="outputs/Screenshot 2026-07-18 214159.png" width="600"><br>
  <img src="outputs/Screenshot 2026-07-18 214252.png" width="600"><br>
  <img src="outputs/Screenshot 2026-07-18 214307.png" width="600"><br>
  <img src="outputs/Screenshot 2026-07-18 214323.png" width="600"><br>
  <img src="outputs/Screenshot 2026-07-18 214334.png" width="600">
</p>

---

## Tech Stack

`Python` · `Pandas` · `NumPy` · `Scikit-learn` · `Matplotlib` · `Seaborn`

## Dataset

Full dataset: [Rossmann Store Sales — Kaggle](https://www.kaggle.com/c/rossmann-store-sales)

`train.csv` is **not included** in this repo (large file, per Kaggle's terms). Download it and place it in `Dataset/`. `store.csv`, `test.csv`, and sample submissions are already included.

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook "Rossman Store Sales.ipynb"
```

## Project Structure

```
Rossman-Store-Sales/
├── Rossman Store Sales.ipynb   # Main analysis & modeling notebook
├── Dataset/                     # Store metadata, test data, sample submissions
├── outputs/                     # Result screenshots
├── requirements.txt
└── README.md
```

---

## Author

**Swapnil Ware**
[LinkedIn](https://www.linkedin.com/) · [GitHub](https://github.com/wareswapnil)
