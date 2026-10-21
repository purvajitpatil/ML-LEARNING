# ML-LEARNING 🤖📈

A public log of my machine learning journey, one day at a time. Each notebook is a small step: load data, explore it, question it, and learn something new.

> *"Day 1: I didn't build a model. I learned to ask the data what it's hiding."*

---

## 📂 Repository Structure

```
ML-LEARNING/
├── ML_day1.ipynb    # Day 1: loading and exploring the medical insurance dataset
└── README.md
```

New days will be added as `ML_dayN.ipynb`, and this README will track the progress.

---

## 📅 Progress Log

| Day | Notebook | Topic | Status |
|-----|----------|-------|--------|
| 1 | [`ML_day1.ipynb`](./ML_day1.ipynb) | Loading data, EDA, distributions | ✅ Done |

---

## 🗓️ Day 1: Exploratory Data Analysis (EDA)

**Goal:** Get comfortable with a real dataset before touching any model.

**Dataset:** A medical insurance dataset with **1,338 records** and **7 features**:

| Column | Type | Description |
|--------|------|-------------|
| `age` | int | Age of the primary beneficiary (18–64) |
| `sex` | categorical | Gender (`male` / `female`) |
| `bmi` | float | Body mass index |
| `children` | int | Number of dependents covered (0–5) |
| `smoker` | categorical | Smoker status (`yes` / `no`) |
| `region` | categorical | US residential region (4 regions) |
| `charges` | float | Individual medical costs billed by insurance (the target) |

> Data source: [stedy/Machine-Learning-with-R-datasets](https://github.com/stedy/Machine-Learning-with-R-datasets)

**What I did:**
- Loaded the dataset with `pandas` straight from a URL
- Inspected shape, dtypes, and summary statistics with `.info()` and `.describe()`
- Checked for missing values (none found ✅)
- Plotted histograms with `seaborn` for `age`, `bmi`, `children`, and `charges` to see how each is distributed

**Key takeaways:**
- The dataset is clean, with no missing values.
- `charges` is right-skewed: most people pay modest amounts, while a few pay much more. This is an important detail for regression later.

---

## 🛠️ Tech Stack

- **Python 3**
- **pandas**, **NumPy**: data handling
- **Matplotlib**, **Seaborn**: visualization
- Runs on **Google Colab** or **Jupyter**

---

## 🚀 How to Run

1. Open `ML_day1.ipynb` in Google Colab, or clone the repo and run it locally:
   ```bash
   git clone https://github.com/purvajitpatil/ML-LEARNING.git
   cd ML-LEARNING
   pip install pandas numpy seaborn matplotlib jupyter
   jupyter notebook ML_day1.ipynb
   ```
2. Run all cells. The dataset downloads automatically, so no manual setup is needed.

---

## 🎯 Roadmap

- [x] Day 1: Data loading & EDA
- [ ] Day 2: Data cleaning & encoding categorical features
- [ ] Day 3: Linear regression to predict `charges`
- [ ] Day 4: Evaluating models (MAE, RMSE, R²)
- [ ] Beyond: Trees, ensembles, and feature importance

---

## 📬 Connect

Learning in public, so feedback and suggestions are welcome. Feel free to open an issue or reach out on GitHub: [@purvajitpatil](https://github.com/purvajitpatil)

⭐ If this helps you start your own ML journey, consider starring the repo!
