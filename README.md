# ✈️ Flight Passenger & Airline Routes Analysis

## 📌 Project Overview

This project explores **airline passenger satisfaction** and **US airline routes/fare data (2020–2024)**.
It combines **EDA, business insights, and predictive modeling** to answer key industry questions:

* What drives passenger satisfaction?
* How do delays, loyalty, and service quality affect sentiment?
* Which routes and carriers dominate high fares?
* Why are some long routes surprisingly cheap?
* Can we predict fares using load factors and distance?

---

## 📂 Datasets

1. **Passenger Satisfaction Data (`train.csv`)**

   * Demographics, travel type, class, service ratings, delays.
   * Target variable: `satisfaction` (0 = dissatisfied/neutral, 1 = satisfied).

2. **US Airline Routes & Fares (1993–2024)**

   * Filtered to **2020–2024**.
   * Includes `city1`, `city2`, `fare`, `nsmiles` (miles), `lf_ms` (load factor), `carrier_lg`.

---

## 🔍 Key Analyses

### 🧑‍🤝‍🧑 Passenger Satisfaction

* **Q1:** Type of Travel → Business travelers are far more satisfied than personal travelers.
* **Q2:** Flight Class → Business class passengers have the highest satisfaction; Economy the lowest.
* **Q3:** Delays → Even short delays reduce satisfaction; long delays crush it.
* **Q4:** Services → WiFi, boarding process, entertainment, seat comfort are top satisfaction drivers.
* **Q5:** Loyalty → Loyal customers report significantly higher satisfaction.

➡️ **Predictive Model:**

* Built a **Random Forest Classifier** with \~96% accuracy.
* Top features: Online boarding, WiFi service, entertainment, seat comfort, cleanliness.

---

### 🛫 US Airline Routes & Fares (2020–2024)

* **Q1:** Top 10 Most Expensive Routes → Premium corridors, likely due to limited competition/business-heavy demand.
* **Q2:** Long Routes with Surprisingly Low Fares → Competition or efficiency keeps fares low despite distance.
* **Q3:** Carriers Dominating High Fares → Certain airlines consistently charge premium fares, reflecting trust or lack of alternatives.

➡️ **Fare Prediction Model:**

* Used **Linear Regression** with `nsmiles` (distance) and `lf_ms` (load factor).
* R² score shows decent accuracy with only 2 features.
* Feature importance: Load factor and distance are primary fare drivers.

---

## 📊 Visual Insights

* Satisfaction by **travel type, class, and delay categories**.
* Correlations of in-flight services with satisfaction.
* Routes sorted by highest fares.
* Long-haul routes sorted by lowest fares.
* Carriers dominating premium pricing.
* Feature importance from models.

---

## 💡 Business Recommendations

1. **Enhance Digital Experience** – Invest in smooth online boarding and booking.
2. **Upgrade Connectivity** – Treat WiFi as a necessity, not an add-on.
3. **Reimagine Economy** – Improve seat comfort and service speed.
4. **Personalize for Leisure Travelers** – Provide offers, bundles, and stress-free experiences.
5. **Build Loyalty** – Reward frequent flyers with perks, upgrades, and consistency.
6. **Fare Optimization** – Use distance and load factor for pricing strategies, while protecting premium routes.

---

## ⚙️ Tech Stack

* **Python**: Data analysis & ML
* **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
* **Models**: Random Forest (classification), Linear Regression (regression)
* **Visualization**: Bar plots, feature importance charts, satisfaction breakdowns

---

## 🚀 How to Run

1. Clone the repo:

   ```bash
   git clone https://github.com/your-username/airline-analysis.git
   cd airline-analysis
   ```
2. Install requirements:

   ```bash
   pip install -r requirements.txt
   ```
3. Run Jupyter Notebook or Google Colab.
4. Load datasets (`train.csv` and `US_Airline_Flight_Routes_and_Fares_1993-2024.csv`).

---

## 📌 Final Takeaway

This project shows how **data-driven analysis can improve customer satisfaction and pricing strategies in the airline industry**.
From **predicting passenger sentiment** to **benchmarking fare strategies**, airlines can use these insights to **balance profitability and customer experience**.


