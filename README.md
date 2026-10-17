# 📊 Titanic Mini Visualization Dashboard — Task 4

### Data Science / Data Analysis with Python Internship — Main Crafts Technology

This repository contains my submission for **Task 4** of the 6-week virtual Data Science internship at **Main Crafts Technology**: a **mini data visualization dashboard** in a single Jupyter Notebook, built with Matplotlib and Seaborn, with a short interpretation under every chart.

---

## 📁 Dataset used

- **Titanic dataset** — [Kaggle: Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic/data)
- **File:** `train.csv` (891 passengers, 12 columns)

---

## 🧱 What the notebook contains

| Section | What happens |
|---|---|
| **Overview** | Goal, dataset and column guide |
| **Cleaning** | `Age` filled with the median, `Embarked` with the mode, `Cabin` dropped |
| **Features** | `FamilySize = SibSp + Parch`, `AgeGroup` (Child → Senior), readable `Outcome` label |
| **Visualizations** | 5 required charts + 1 bonus facet grid, each with a 1–2 line insight |
| **Insights** | Summary table of takeaways |
| **Conclusion** | Overall findings and limitations |

### Dashboard charts

| # | Chart type | What it shows |
|---|---|---|
| 1 | Histogram | Age distribution |
| 2 | Bar chart | Survival rate by class and gender |
| 3 | Boxplot | Fare distribution by class (with outliers) |
| 4 | Scatterplot | Age vs Fare, coloured by survival |
| 5 | Heatmap | Correlations between numeric columns |
| 6 | Facet grid (bonus) | Survival by age group, split by gender |

All charts are exported as PNGs to the [`images/`](images/) folder.

---

## 🔍 Key Insights

- 👩 Women survived far more than men in **every** class (97% vs 37% in 1st class, 92% vs 16% in 2nd, 50% vs 14% in 3rd). Even 3rd-class women (50%) beat 1st-class men (37%).
- 💷 Median fares fall from ~60 (1st) to ~14 (2nd) to ~8 (3rd); 1st class has extreme outliers up to 512.
- 🎟️ Passengers paying over 100 survived ~74% of the time vs ~36% for the rest, though age and fare themselves are almost unrelated.
- 👦 Among men, only boys had good survival odds (~57%); teenage and adult men survived at just 9–23%.

---

## 📂 Repository structure

```
├── README.md
├── Titanic_Dashboard_Task4.ipynb    # final single notebook (main deliverable)
├── data/
│   └── train.csv                    # download from Kaggle (see below)
├── images/                          # exported charts (.png)
└── notebooks/                       # day-wise progress versions
    ├── Day1_Overview_and_Loading_Task4.ipynb
    ├── Day2_Cleaning_and_Features_Task4.ipynb
    ├── Day3_Charts_1_2_Task4.ipynb
    ├── Day4_Charts_3_to_5_and_Bonus_Task4.ipynb
    └── Day5_Insights_and_Conclusion_Task4.ipynb
```

---

## 🚀 How to Run

1. Clone this repository.
2. Download `train.csv` from the [Kaggle Titanic page](https://www.kaggle.com/c/titanic/data) and place it in the `data/` folder (or skip this and upload it when prompted in Colab).
3. Open `Titanic_Dashboard_Task4.ipynb` in [Google Colab](https://colab.research.google.com/) or Jupyter.
4. Run all cells. The notebook looks for the file in `data/` first, then the working folder, and prompts for an upload in Colab if it is not found.

**Requirements:** `pandas`, `numpy`, `matplotlib`, `seaborn`.

---

## ⚠️ Limitations

Missing ages were filled with the median, which creates an artificial spike at 28 in the age histogram. Some subgroups (seniors, very large families) are small, so their rates are less reliable.

---

*Completed as part of the 6-week virtual internship at **Main Crafts Technology**.*

#DataScience #Python #Seaborn #Matplotlib #DataVisualization #TechInternship #Maincrafts
