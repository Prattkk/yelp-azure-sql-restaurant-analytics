# 🍽️ Yelp Restaurant Location & Concept Strategy

This project is an end-to-end analytics case study using the **Yelp Open Dataset** to support a real business decision:
**Where should I open a restaurant, what type should it be, and why?**

The work combines **SQL-based business analysis** with a **Python-only interactive Marimo application**.

---

## 🎯 Business Objective
Opening a restaurant involves high risk and capital investment. Using real Yelp data, this project evaluates:
- Market saturation & competition
- Customer preferences and complaints
- Opportunity gaps by location and cuisine

to recommend a **data-backed restaurant concept and target location**.

---

## 📊 Data Understanding
- Dataset: Yelp Open Dataset (JSON format)
- Entities analyzed:
  - Businesses
  - Reviews
  - Users
  - Check-ins
  - Tips
- Explored:
  - Nested JSON structures
  - Geographic coverage (city/state)
  - Review time period and volume

All exploration and analysis are documented in the notebook.

---

## 🧠 Business Analysis (SQL)
Using SQL queries, the notebook answers strategic questions such as:
- Where is the restaurant market most saturated?
- Which cuisines perform best at different price points?
- What factors correlate with high ratings and review volume?
- What common complaints appear in low-rated restaurants?
- Which areas show **high demand but limited competition**?

Each query is tied to a **business decision**, not just technical output.

---

## 🐍 Python-Only Extension (Marimo)
To extend the project beyond SQL, I rebuilt the analysis using **Python only (no SQL)** and published it as a **Marimo interactive web app**.

### Interactive Features
- City-level filtering
- Cuisine / category selection
- Dynamic recalculation of insights based on user input

This demonstrates the ability to translate SQL logic into Python analytics workflows.

---

## 📁 Repository Structure


---

## ▶️ Files
- `notebook/yelp_analysis.ipynb`  
  → Data exploration and SQL-based business insights
- `app/marimo_app.html`  
  → Python-only interactive analytics application
- `app/marimo_screenshot.png`  
  → Screenshot demonstrating interactivity

---

## 🛠️ Tech Stack
- SQL (Azure SQL)
- Python (pandas, JSON processing)
- Kaggle / Google Colab
- Marimo (interactive analytics)

---

## 👤 Author
**Prateek Verma**  
MS in Business Analytics, UIUC (Gies College of Business)
