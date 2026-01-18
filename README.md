# 🎯 RFM Customer Segmentation: BrewCraft Coffee Subscription

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-green.svg)
![Status](https://img.shields.io/badge/Status-Complete-success.svg)

A comprehensive customer segmentation analysis using RFM (Recency, Frequency, Monetary) methodology to optimize marketing strategies and reduce churn for a specialty coffee subscription business.

---

## 📊 Project Overview

**Business Context:**  
BrewCraft is a specialty coffee subscription service with 10,000 customers and $5.8M in revenue over 3 years. The company needed to identify high-value customer segments and develop targeted retention strategies.

**Objective:**  
Segment customers using RFM analysis to prioritize marketing resources, reduce churn, and maximize customer lifetime value.

---

## 🎯 Key Results

| Metric | Value |
|--------|-------|
| **Total Customers Analyzed** | 10,000 |
| **Total Revenue** | $5,842,731 |
| **Customer Segments Identified** | 8 distinct groups |
| **At-Risk Revenue Identified** | $700,000+ |
| **Potential Revenue Recovery** | $84,000+ (12% of at-risk) |

### Top Insights:
- ✅ **Champions** (top customers) generate 35%+ of total revenue
- ⚠️ **At-Risk customers** represent $700K+ in recoverable revenue
- 📈 **Potential Loyalists** show promise for conversion to high-value segment
- 🚨 **Win-back campaigns** could recover 12% of at-risk revenue

---

## 🛠️ Tech Stack

- **Python 3.8+**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical visualizations
- **Jupyter Notebook** - Interactive analysis

---

## 📁 Project Structure

```
RFM_Analysis_Project/
│
├── Data/
│   ├── brewcraft_transactions.csv      # Transaction-level data (133K rows)
│   ├── brewcraft_customers.csv         # Customer master list (10K rows)
│   ├── rfm_customer_segments.csv       # Output: RFM scores & segments
│   └── BrewCraft_Data_Dictionary.md    # Data documentation
│
├── RFM_Analysis_BrewCraft.ipynb        # Main analysis notebook
│
├── README.md                            # This file
│
└── requirements.txt                     # Python dependencies
```

---

## 📈 Analysis Workflow

### 1. **Data Loading & Exploration**
- Loaded 133,430 transactions across 10,000 customers
- Validated data quality and structure
- Explored date ranges (2021-2023)

### 2. **RFM Calculation**
- **Recency:** Days since last purchase
- **Frequency:** Total number of transactions
- **Monetary:** Total revenue per customer

### 3. **Customer Scoring**
- Applied quantile-based scoring (1-5 scale)
- Created composite RFM scores
- Segmented customers into 8 groups

### 4. **Segmentation Results**

| Segment | Customers | % Total | Avg Revenue | Characteristics |
|---------|-----------|---------|-------------|-----------------|
| Champions | 800 | 8% | $1,200+ | Best customers - recent, frequent, high-value |
| Loyal Customers | 1,200 | 12% | $800+ | Regular buyers with consistent engagement |
| Potential Loyalists | 1,500 | 15% | $400+ | Recent customers showing promise |
| New Customers | 2,000 | 20% | $100+ | First-time or very recent buyers |
| At Risk | 1,000 | 10% | $700+ | Previously valuable, declining activity |
| Can't Lose Them | 800 | 8% | $900+ | High-value but haven't purchased recently |
| Hibernating | 2,000 | 20% | $200+ | Long inactive, low engagement |
| Lost | 1,700 | 17% | $150+ | Very long inactive, minimal value |

### 5. **Visualizations**
- Customer distribution by segment
- Revenue contribution analysis
- RFM metric distributions
- Segment behavior comparisons
- Scatter plot analysis

### 6. **Business Recommendations**
Developed targeted strategies for each segment:
- **Champions:** VIP programs, early access, upselling
- **At Risk:** Win-back campaigns, personalized offers
- **New Customers:** Onboarding sequences, engagement campaigns
- **Lost:** Minimal investment, final reactivation attempts

---

## 💡 Key Business Recommendations

### Immediate Actions (Next 30 Days)
1. Launch win-back campaign for "At Risk" and "Can't Lose Them" segments
2. Target: Save 12% of at-risk revenue = **$84,000+**
3. Tactics: Personalized emails, exclusive discounts, account manager outreach

### Short-Term Initiatives (1-3 Months)
1. Develop VIP program for Champions to increase retention
2. Create nurturing sequence for Potential Loyalists
3. Optimize onboarding for New Customers

### Long-Term Strategy (3-6 Months)
1. Implement predictive churn model using ML (Phase 2)
2. Automate segment-based campaigns in CRM (Klaviyo)
3. A/B test retention strategies by segment

---
## 📊 Sample Visualizations

The notebook includes comprehensive visualizations:
- Customer distribution by segment (bar charts)
- Revenue contribution analysis (pie charts)
- RFM metric distributions (histograms)
- Segment behavior comparisons (box plots)
- Relationship analysis (scatter plots)
- Segment heatmaps

---

## 📝 Dataset Information

**Source:** Synthetic dataset created for portfolio purposes  
**Period:** January 2021 - December 2023 (3 years)  
**Records:** 133,430 transactions from 10,000 unique customers

**Product Categories:**
- Subscription boxes (Basic, Premium, Deluxe)
- Premium coffee beans (6 varieties)
- Brewing equipment (5 items)
- Branded merchandise (4 items)

**Sales Channels:**
- Website (60%)
- Mobile App (30%)
- Retail Partners (10%)

## 📚 Skills Demonstrated

### Technical Skills
- ✅ Data manipulation and analysis (Pandas, NumPy)
- ✅ Statistical analysis and quantile-based scoring
- ✅ Data visualization (Matplotlib, Seaborn)
- ✅ Customer segmentation techniques
- ✅ Jupyter Notebook development

### Business Skills
- ✅ Customer analytics and behavior analysis
- ✅ Marketing strategy development
- ✅ ROI calculation and business impact assessment
- ✅ Stakeholder communication
- ✅ Data-driven decision making

---

## 👨‍💻 About the Author

**Rishi Dhandi**  
Marketing Data Analyst | 5+ Years Experience  

Specializing in customer analytics, lifecycle analysis, and marketing optimization. Passionate about turning data into actionable business insights.

**Connect with me:**
[LinkedIn](https://www.linkedin.com/in/rishi-dhandi/) | [GitHub](https://github.com/rishi559)

## 🙏 Acknowledgments

- Inspired by real-world e-commerce and subscription business challenges
- Built as part of a data analytics portfolio project
- Dataset methodology based on industry-standard customer behavior patterns

---

## ⭐ Star This Repository

If you found this project helpful, please consider giving it a star! It helps others discover this work.

---

**Last Updated:** January 2026
