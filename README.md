# Airbnb-Anomaly-Detection

A data-driven project that enhances **trust and safety** on Airbnb by identifying suspicious listings through **Machine Learning (ML)** and **Natural Language Processing (NLP)**.  
Combines **Isolation Forest**, **DBSCAN**, and **Sentiment Analysis** to detect anomalies in pricing, reviews, and availability — producing a composite **Trust Score** for each listing.  


## Problem Statement  

Airbnb listings often contain misleading information — from fake reviews and manipulated prices to inconsistent availability. These patterns affect guest trust and booking confidence.  
This project applies **unsupervised learning and sentiment analysis** to detect potential fraud and quantify listing reliability with a **Trust Score (0–1)**.


## Objective  

To design a **Trust Scoring Framework** using ML and NLP that identifies and quantifies suspicious Airbnb listings by analyzing patterns in:
- Pricing fluctuations  
- Host behaviors  
- Review sentiment  
- Availability inconsistencies


## 📁 Datasets  

Data sourced from **Inside Airbnb’s open datasets**

- **listings.csv** – Property-level details  
- **calendar.csv** – Daily prices and availability  
- **reviews.csv** – Review metadata and text
 > Due to size constraints, datasets are not uploaded here. Please download publicly available data or use small samples


## Approach  
1. **Data Cleaning & Feature Engineering** – Processed Airbnb `listings`, `calendar`, and `reviews` datasets.  
2. **Anomaly Detection (ML)** – Used **Isolation Forest** and **DBSCAN** to detect outliers in price, review count, and availability.  
3. **Sentiment Analysis (NLP)** – Applied **VADER** to analyze review text and compute sentiment scores.  
4. **Trust Score Calculation** – Combined ML and NLP outputs into a composite metric

## Results  
- Detected **774 anomalous listings** (~5% of dataset).  
- Identified **low-trust** listings with multiple red flags (pricing, reviews, sentiment).  
- Created **heatmaps** and **distribution plots** to visualize anomalies and trust levels.


## Visualizations  
- **Heatmaps:** Show concentration of low-trust listings in certain city zones.
- **Boxplots:** Compare sentiment scores of anomalous vs normal listings.  
- **Distribution Plots:** Highlight pricing outliers and review anomalies.

## Outcome  
- Enhanced Airbnb data reliability by flagging anomalies and low-trust listings.  
- Developed a **Trust Scoring Framework** for prioritizing suspicious properties.  
- Combined **ML + NLP + Rule-based logic** for a anomaly detection pipeline.  


## Technologies Used  

| Category | Tools & Libraries |
|-----------|------------------|
| **Languages** | Python |
| **Libraries** | Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, NLTK |
| **Models** | Isolation Forest, DBSCAN, VADER Sentiment |
| **Visualization** | Matplotlib, Seaborn, Folium |
| **Environment** | Jupyter Notebook |

