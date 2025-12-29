# Amazon Bestselling Books Analysis (2009–2019)

## 📌 Project Overview

This project is an end-to-end data analysis case study examining the characteristics of books that become and remain Amazon Top 50 Bestsellers.

Using historical bestseller data from 2009 to 2019, the analysis explores how **genre**, **pricing**, **user ratings**, **review volume**, and **author persistence** relate to sustained bestseller performance.

The project follows the full analytics lifecycle:

**Ask → Prepare → Process → Analyse → Share → Act**

and is designed as a **portfolio-ready case study** targeting Junior / Experienced Junior Data Analyst roles.

---

## ❓ Business Question

**What characteristics are most strongly associated with books becoming and remaining Amazon bestsellers, based on price, genre, user ratings, and review volume?**

---

## 📊 Dataset

- **Source:** Amazon Top 50 Bestselling Books (2009–2019)
- **Provider:** Kaggle (public dataset)
- **Records:** Annual Top 50 books across 11 years
- **Key fields:**
  - Book name
  - Author
  - Genre (Fiction / Non-Fiction)
  - Price
  - User rating
  - Number of reviews
  - Year

Raw data is stored in `data_raw/` and excluded from version control.  
Cleaned data is saved to `data_cleaned/` and used for analysis.

---

## 🧭 Project Structure


├── notebooks/
│ ├── 01_define_problem_and_prepare.ipynb
│ ├── 02_load_and_clean.ipynb
│ ├── 03_analysis.ipynb
│ ├── 04_visuals_for_report.ipynb
│ └── 05_recommendations_and_next_steps.ipynb
│
├── data_raw/ # Raw data (git-ignored)
├── data_cleaned/ # Cleaned datasets
├── reports/ # Report-ready visuals (PNG)
│
├── requirements.txt
└── README.md

---

## 🔍 Key Insights

### 1️⃣ Genre dominance
- Bestseller lists are not evenly distributed by genre.
- One genre consistently represents a larger share of Top 50 titles.
- Genre composition remains relatively stable over time.

![Genre Share Over Time](reports/genre_share_over_time.png)  
![Overall Genre Share](reports/overall_genre_share.png)

---

### 2️⃣ Pricing follows a narrow “bestseller band”
- Bestsellers cluster around a limited range of price points.
- Pricing norms differ slightly by genre but remain consistent over time.

![Price Distribution by Genre](reports/price_distribution_by_genre.png)

---

### 3️⃣ Popularity vs satisfaction
- High user ratings are common across bestsellers.
- Review volume varies widely and acts as a strong popularity signal.
- The strongest-performing books combine **high ratings and high review volume**.

![Rating vs Reviews](reports/rating_vs_reviews.png)

---

### 4️⃣ Author persistence reduces risk
- Some authors appear repeatedly across multiple years.
- Repeat appearances indicate sustained demand and lower uncertainty.

![Top Repeat Authors](reports/top_repeat_authors.png)

---

## 💡 Business Recommendations

- **Prioritise dominant genres** when allocating marketing and acquisition budgets.
- **Use historical bestseller price bands** to inform pricing strategy.
- **Monitor early performance indicators** (rating + review velocity) for new releases.
- **Build partnerships with repeat authors** to reduce launch risk.
- **Improve ethical review-generation strategies** to support visibility and ranking.

---

## ⚠️ Limitations

- Sales volume is not available; reviews are used as a proxy for popularity.
- The dataset includes only Top 50 books per year, not the full catalogue.
- Relationships observed are associative, not causal.

---

## 🔧 Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebooks
- GitHub / Codespaces

---

## 📌 Status

**Completed — Portfolio Ready**

This project demonstrates:
- Structured problem framing
- Data cleaning and validation
- Business-focused analysis
- Clear communication of insights
- Actionable recommendations
