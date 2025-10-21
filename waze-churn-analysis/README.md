# 🛣️ Waze User Churn Analysis

This project was completed as part of the **Google Advanced Data Analytics Certificate (Course 3)**. It focuses on identifying behavioral patterns in Waze app users that correlate with churn, using exploratory data analysis (EDA), visualization, and feature engineering in Python.

---

## Project Goals

- Explore and clean user-level activity data from Waze
- Visualize behavioral differences between retained and churned users
- Identify early indicators of churn (e.g. session spikes, driving intensity)
- Communicate results in the form of an executive summary

## Executive Summary
Analysis of 15,000+ Waze users revealed that **churners drove less frequently 
but more intensely** (600+ km/day). 42% of their sessions occurred in the 
final month, indicating detectable early warning signals. Recommended: 
targeted onboarding for new users and activity-based churn risk scoring.

---

## Repository Structure

```
waze-churn-analysis/
├── activity_course3.ipynb        # Jupyter Notebook with full EDA
├── visuals/                      # Exported PNGs of key visualizations
└── README.md                     # Project overview & summary
```

---

## Key Visualizations

### Histogram of Sessions  
![Histogram of Sessions](visuals/hist_sessions.png)

### Histogram of Drives  
![Histogram of Drives](visuals/hist_drives.png)

### Histogram of Driven Kilometers (Monthly)  
![Histogram of KM](visuals/hist_km_monthly.png)

### Retained vs Churned Distribution  
![Churn Pie](visuals/pie_churn_status.png)

### User Retention by Device  
![Device Retention](visuals/bar_retention_device.png)

### Churn vs Retention by Kilometers per Driving Day  
![Churn vs KM](visuals/hist_km_per_day_churn.png)

### Churn Rate per Number of Driving Days  
![Churn by Driving Days](visuals/hist_driving_days_churn.png)

### Distribution of Percent of Sessions in Last Month  
![Percent Sessions Last Month](visuals/hist_percent_sessions_last_month.png)

---

## Summary of Key Insights

- **Churners drove less frequently**, but covered more kilometers per driving day
- Over **42% of their sessions occurred in the final month**
- Churn was **most common among newer users**
- Churn rates were **consistent across device types**

---

## Business Recommendations

- Send personalized onboarding nudges in weeks 1–2
- Flag high-risk users with session spikes or >600 km/day driving
- Investigate long-tenure users with sudden activity bursts before churn
- Develop a churn-risk score using usage intensity & lifetime behavior

---

## Tools & Techniques

- Python: `pandas`, `seaborn`, `matplotlib`
- Jupyter Notebook for analysis & commentary
- Feature creation: `km_per_driving_day`, `percent_sessions_in_last_month`
- Outlier handling (95th percentile), histogram-based ratio comparison

---

## Author

**Jonatan Zemedebrhan**  
Google Advanced Data Analytics Certificate – Course 3  
Waze User Churn Case Study

---

⚠️ **To run this notebook locally**, make sure the file  
`waze_data.csv` is placed in the **same folder** as the notebook.  
This dataset was originally generated inside the Coursera platform and is included in this repository for reproducibility.

