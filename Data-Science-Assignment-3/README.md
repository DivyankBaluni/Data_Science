# 🌍 Global Terrorism Analysis (UNGTA Dataset)

## 📌 Project Overview

This project performs a comprehensive **Exploratory Data Analysis (EDA)** on the United Nations Global Terrorism Analysis (UNGTA) dataset. Spanning from **1970 to 2017**, the dataset contains over **180,000 recorded terrorist incidents** worldwide.

The objective is to **clean, process, and visualize** the data to extract actionable insights into the evolving landscape of global terrorism, identifying trends in geography, tactics, and lethality.

---

## 🎯 Objectives

* 📂 Load and inspect the UNGTA dataset (180,000+ rows)
* 🧹 Handle missing values and drop analytically irrelevant columns
* 🔄 Clean and rename features for better interpretability
* ➕ Engineer new features (e.g., *total_casualties*, *lethality_index*, *decade*)
* 📊 Perform Univariate, Bivariate, and Multivariate EDA
* 📉 Apply statistical hypothesis testing (t-test, Chi-square)
* 💡 Generate data-driven recommendations for security stakeholders

---

## 🛠️ Tools & Technologies

* 🐍 Python
* 🐼 Pandas
* 🔢 NumPy
* 📉 Matplotlib
* 🎨 Seaborn

---

## 🧼 Data Cleaning

The dataset was preprocessed using the following steps:

* 🗑️ Filtered 135 columns down to 23 analytically relevant variables
* ⚠️ Handled high null percentages (dropped columns > 60% missing)
* 🔧 Renamed cryptic column names (e.g., `nkill` → `killed`, `iyear` → `year`)
* ➕ Created a **`casualties`** column (`nkill + nwound`)
* 📅 Extracted additional features such as:
  * **Decade** & **Decade Label** 
  * **Month** 
  * **Decade** 

---

## 📌 Key Features Used

* 📅 `year`, `month`, `day`
* 🌍 `country`, `region`, `provstate`, `city`
* 💣 `attack_type`
* 🎯 `target_type`, `target_subtype`
* 👥 `gname` (Terrorist Group)
* 🔫 `weapon_type`
* ☠️ `killed`, 🤕 `wounded`
* ✅ `success`, ⚔️ `suicide`
* 📊 `total_casualties`, `lethality_index` (engineered)

---

## 📊 Exploratory Data Analysis

The analysis focuses on:

* 📈 Temporal trends: Identifying the global peak in terrorism (2014)
* 🌍 Geographic concentration: Analyzing most affected countries (Iraq, Pakistan, Afghanistan)
* 💣 Tactic analysis: Dominance of Bombings and Explosives
* 🎯 Target profiles: Comparing "Soft" vs. "Hardened" targets
* ☠️ Lethality assessment: Impact of suicide attacks vs. non-suicide attacks
* 🔗 Correlation analysis: Relationships between weapon types, casualties, and success rates

---

## 📉 Visualizations

* 📈 Line chart: Number of attacks per year (1970–2017)
* 📊 Bar chart: Top 10 countries and regions by attack volume
* 🍩 Donut chart: Distribution of attack types
* 🔥 Heatmap: Attacks by Region vs. Decade
* 🗺️ Stacked Area Chart: Proportion of global attacks by region over time
* 📦 Box plot: Casualty distribution across different world regions
* 📉 Bubble Scatter: Group attack frequency vs. average lethality
* 🔥 Heatmap: Correlation matrix of numeric features

---

## 💡 Key Insights

* 🌍 Terrorism surged post-2001, peaking in **2014** due to regional instabilities and the rise of ISIS.
* 📍 **Iraq**, **Pakistan**, and **Afghanistan** bear a disproportionate burden of global incidents.
* 💣 **Bombing/Explosion** is the most frequent attack method (~50% share).
* ☠️ **Suicide attacks** are statistically significantly more lethal than non-suicide attacks (p < 0.05).
* 🎯 **Target Hardening** works: Military and Government targets have lower success rates compared to softer targets.
* 🧠 Threat centers shift over decades—Western Europe peaked in the 80s, while the Middle East dominated the 2010s.

---

## 👥 Stakeholder Relevance

This analysis can benefit:

* 🏛️ **Government Agencies** for strategic planning and counter-terrorism resource allocation.
* 🛡️ **Security Organizations** for identifying high-risk tactics and regional threat levels.
* 🚑 **Emergency Services** for calibrating response surge capacity based on regional lethality signatures.
* 🎓 **Researchers** for studying the lifecycle and impact of terrorist organizations.
* 🌐 **International NGOs** for risk assessment in conflict zones.

---

## 📁 Project Structure

```
project-folder/
│── UNGTA_Global_Terrorism_Analysis.ipynb    # Main Analysis Notebook
│── globalterrorismdb.csv                    # Dataset (to be added)
│── README.md                                # Project Documentation
└── images/                                  # Exported Visualizations
```

---

## 🚀 Getting Started

1. 📥 Clone the repository `git clone https://github.com/your-username/global-terrorism-analysis.git`
2. 💻 Open `UNGTA_Global_Terrorism_Analysis.ipynb` in Jupyter Notebook, or Google Colab.
  (or `Data`)
3. 📦 Install required libraries (if needed)
4. ▶️ Run the notebook cells sequentially to reproduce the cleaning, analysis, and visualizations.

---

## 🏁 Conclusion

This analysis demonstrates how data cleaning and exploratory visualization can uncover the underlying patterns of global conflict. By identifying high-risk regions, typical attack vectors, and the factors influencing lethality, we can provide data-driven insights that are crucial for modern security and policy-making.

---

## ✍️ Author

**Divyank Baluni**
