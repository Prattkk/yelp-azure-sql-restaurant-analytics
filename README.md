# 🍽️ Yelp Restaurant Location & Concept Strategy (Azure SQL + Python)

End-to-end analytics case study using the Yelp Open Dataset to support a restaurant launch decision:
**JSON → Azure SQL relational database → 10+ strategic SQL insights → Python-only interactive Marimo web app (no SQL).**

---

## 🎯 Business Question
If I were opening a new restaurant, **which city/area should I target, what concept should I launch, and how do I differentiate**, using real customer and competitor data from Yelp?

---

## 🧱 What I Built
### ✅ Milestone 1 — Data Understanding (Yelp JSON)
- Explored Yelp semi-structured JSON files (business, reviews, users, check-ins, tips)
- Documented nested fields, data types, geography, and review time period
- Notebook (Kaggle/Colab) explains dataset scope and transformation plan

### ✅ Milestone 2 — Database Implementation (Azure SQL)
- Designed and implemented a relational schema in **Azure SQL Server**
- Converted JSON → structured SQL tables with:
  - Primary keys / foreign keys
  - Data types and constraints
  - Validation checks to confirm completeness and correctness
- Verified metadata against a reference `yelp_champaign` database

### ✅ Milestone 3 — Business Insights (SQL)
Wrote **10+ SQL queries** that inform real decisions:
- Market saturation & competition analysis
- High-demand / low-competition opportunity zones
- Rating + review volume competitive benchmarks
- Customer preferences & complaint patterns
- Differentiation levers (amenities, price range, cuisine)

### ⭐ Extra Credit — Python-Only (Marimo Web App)
Rebuilt the analysis with **Python only (no SQL)** and published a **Marimo interactive app**:
- Replicated joins/aggregations in Python
- Added interactive filters (city, cuisine/category, price range, rating thresholds)

---

## 🗂️ Repository Contents
- `sql/` → schema + constraints + validation + business insight queries
- `notebooks/` → Kaggle/Colab notebook link + optional exported notebook
- `app/` → Marimo interactive Python app + requirements
- `docs/` → ERD, diagrams, and screenshots

---

## 🏗️ Database Schema (High Level)
Main tables:
- `business`
- `review`
- `user`
- `checkin`
- `tip`

See: `docs/erd.png` and `sql/01_schema.sql`

---

## 🔍 Business Insights (Examples)
A few questions answered by SQL:
1. Which neighborhoods/cities have **high demand but low competition**?
2. What cuisines perform best at each price tier?
3. What factors correlate with high ratings (e.g., delivery, reservations, parking)?
4. What are top complaint themes in low-rated restaurants?

All queries: `sql/04_business_queries.sql`

---

## 🛠️ Tech Stack
- **SQL**: Azure SQL Server
- **Python**: pandas / json processing
- **Platform**: Kaggle / Google Colab
- **Interactive App**: Marimo
- **Data**: Yelp Open Dataset (JSON)

---

## ▶️ How to Run the Marimo App (Python-only)
```bash
cd app
pip install -r requirements.txt
marimo run marimo_app.py
