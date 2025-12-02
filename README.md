# 10 Academy – AI Mastery Program  
## Week 2 Challenge: Customer Experience Analytics for Fintech Apps  

**Project:** Scraping, Analyzing, and Visualizing Google Play Store Reviews for Ethiopian Banks  
**Date:** 26 Nov – 02 Dec 2025  

---

## 🎯 Challenge Overview

This project simulates a real-world data engineering and analytics task. You act as a **Data Analyst at Omega Consultancy**, supporting three Ethiopian banks:

- Commercial Bank of Ethiopia (CBE)  
- Bank of Abyssinia (BOA)  
- Dashen Bank  

**Objective:** Scrape user reviews from Google Play, preprocess text, analyze sentiment and themes, visualize insights, and deliver actionable recommendations to improve mobile app performance and user satisfaction.

**Focus Areas:**  

- **User Retention:** Identify common complaints (e.g., slow transfers) and patterns in ratings.  
- **Feature Enhancement:** Extract desired features and improvement requests from reviews.  
- **Support Efficiency:** Cluster complaints to guide support strategies, including AI chatbot integration.  

---

## 🗂 Dataset Overview

- **Source:** Google Play Store  
- **Fields Collected:**  
  - `review_text` → User feedback  
  - `rating` → 1–5 stars  
  - `review_date` → Date of review  
  - `bank_name` / `app_name` → Bank identifier  
  - `source` → Google Play  
- **Minimum Reviews:** 400 per bank (1,200 total)  

---

## 🚀 Project Tasks & Deliverables

### **Task 1: Data Collection & Preprocessing**
- **Web Scraping:** Use `google-play-scraper` or BeautifulSoup to collect reviews.  
- **Preprocessing:** Remove duplicates, normalize dates, clean text (remove emojis, URLs, stopwords).  
- **Deliverables:**  
  - Cleaned CSV with columns: `review`, `rating`, `date`, `bank`, `source`  
  - GitHub repo with organized commits in **task-1** branch  

**KPIs:** ≥1,200 reviews, <5% missing data, properly committed scripts  

---

### **Task 2: Sentiment & Thematic Analysis**
- **Sentiment Analysis:** Compute sentiment scores (positive/negative/neutral) using VADER, TextBlob, or a transformer model.  
- **Thematic Extraction:**  
  - Extract keywords (TF-IDF or regex-based)  
  - Cluster into 3–5 themes per bank (e.g., UI, Reliability, Customer Support)  
- **Deliverables:** CSV with `review_id`, `review_text`, `sentiment_label`, `sentiment_score`, `themes`  

**KPIs:** Sentiment scores for ≥90% of reviews, ≥3 themes per bank  

---

### **Task 3: Store Cleaned Data in PostgreSQL**
- **Database Setup:**  
  - Create `bank_reviews` database  
  - Tables: `banks` and `reviews` with proper keys and constraints  
- **Data Insertion:** Use Python (`psycopg2` or `SQLAlchemy`)  
- **Deliverables:** Working database with >1,000 reviews, schema documented in README  

---

### **Task 4: Insights & Recommendations**
- **Analysis:** Identify key drivers (e.g., speed) and pain points (e.g., crashes) per bank  
- **Visualization:** 3–5 plots (sentiment trends, rating distributions, keyword clouds)  
- **Recommendations:** Actionable improvements per bank  

**KPIs:** ≥2 drivers/pain points per bank, stakeholder-ready visualizations  

---

## 📂 Project Structure




