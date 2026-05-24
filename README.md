# Barcelona FC Players Fitness & Performance Analytics

An end-to-end Sports Data Science project that leverages Machine Learning and advanced statistical analysis to monitor, evaluate, and predict the fitness levels and performance metrics of football players. 

---

## Project Overview
In modern football, data analytics plays a pivotal role in injury prevention, tactical planning, and workload management. This project analyzes athletic data, physical metrics, and performance indicators to uncover insights into player fitness and build predictive models that help optimize squad performance and scouting reports.

## Technical Skills & Tools
* **Language:** Python
* **Environment:** Jupyter Notebook
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn

---

## Data Pipeline & Methodology

### 1. Exploratory Data Analysis (EDA) & Sports Metrics
* Analyzed player profiles, field positions, physical attributes, and workload distributions.
* Visualized correlation matrices to understand the relationship between training loads, passing accuracy, and overall player performance.
* Filtered and benchmarked metrics ensuring players with realistic match minutes ($\ge 90$ mins) are analyzed.

### 2. Feature Engineering & Custom Benchmarking
* Handled missing metrics and standardized physical/tactical performance values.
* Engineered a custom sports-specific classification feature (`Barca_Fit`) based on explicit performance thresholds:
  * **Elite Level (Class 0):** High passing accuracy ($\ge 90\%$), elite volume ($\ge 150$ passes), and defensive contribution ($\ge 3$ tackles won).
  * **Standard Level (Class 1):** Solid metrics ($\ge 80\%$ accuracy and $\ge 80$ passes).
  * **Sub-optimal Level (Class 2):** Below benchmark metrics.

### 3. Predictive Modeling & Scouting Automation
* Grouped and sorted player performance data to automate advanced scouting reports.
* Generated data-driven shortlists ranking elite profiles by workload volume, providing a quantitative framework to evaluate squad depth and transfer targets.

---

## Repository Structure
```text
├── Barca fit players Project.ipynb # Full Jupyter Notebook with sports analytics pipeline
└── README.md                       # Project documentation (This file)
