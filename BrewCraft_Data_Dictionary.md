# BrewCraft Coffee Subscription - RFM Analysis Dataset

## 📊 Dataset Overview

**Business Context:** BrewCraft is a specialty coffee subscription service offering premium coffee beans, brewing equipment, and branded merchandise through multiple sales channels.

**Dataset Period:** January 1, 2021 - December 31, 2023 (3 years)

**Key Metrics:**
- **Total Customers:** 10,000
- **Total Transactions:** 133,430
- **Total Revenue:** $5,842,731.19
- **Average Order Value:** $43.79

---

## 📁 Files Included

### 1. brewcraft_transactions.csv
Main transaction-level dataset containing all customer purchases.

**Columns:**

| Column Name | Data Type | Description | Example |
|------------|-----------|-------------|---------|
| `transaction_id` | String | Unique identifier for each transaction | TXN00100000 |
| `customer_id` | String | Unique identifier for each customer | CUST001000 |
| `transaction_date` | Date | Date of purchase (YYYY-MM-DD) | 2023-10-20 |
| `product_name` | String | Name of product purchased | Premium Monthly Box |
| `product_category` | String | Product category | Subscription, Coffee, Equipment, Merchandise |
| `quantity` | Integer | Number of items purchased | 1, 2, 3 |
| `unit_price` | Float | Price per unit ($) | 49.99 |
| `total_amount` | Float | Total transaction amount ($) | 149.97 |
| `channel` | String | Sales channel | Website, Mobile App, Retail Partner |
| `customer_segment` | String | Original customer segment (for reference) | Champions, Loyal, At Risk, etc. |

**Record Count:** 133,430 rows

---

### 2. brewcraft_customers.csv
Customer master list with original segment classification.

**Columns:**

| Column Name | Data Type | Description | Example |
|------------|-----------|-------------|---------|
| `customer_id` | String | Unique identifier for each customer | CUST001000 |
| `original_segment` | String | Pre-classified segment (for validation) | Champions |

**Record Count:** 10,000 rows

**Note:** The `original_segment` field is included for validation purposes. Your RFM analysis should calculate segments independently from the transaction data.

---

## 🎯 RFM Analysis Objectives

### Key Questions to Answer:

1. **Customer Segmentation**
   - How many customers fall into each RFM segment?
   - What are the characteristics of each segment?
   - Which segments generate the most revenue?

2. **Customer Behavior**
   - What is the purchase frequency distribution?
   - What is the average customer lifetime value by segment?
   - Are there seasonal patterns in purchases?

3. **Business Insights**
   - Which customer segments are at risk of churning?
   - What products do high-value customers prefer?
   - How do different sales channels perform?

4. **Marketing Recommendations**
   - What retention strategies should be applied to each segment?
   - Where should marketing resources be allocated?
   - Which customers have potential for upselling?

---

## 📈 Product Catalog

### Subscriptions (Monthly recurring)
- **Basic Monthly Box:** $29.99
- **Premium Monthly Box:** $49.99
- **Deluxe Monthly Box:** $69.99

### Coffee Beans (Individual bags)
- Ethiopian Yirgacheffe: $18.99
- Colombian Supremo: $16.99
- Sumatra Mandheling: $19.99
- Costa Rican Tarrazu: $17.99
- Guatemala Antigua: $18.49
- Kenya AA: $21.99

### Equipment
- Pour Over Set: $45.00
- French Press: $35.00
- Burr Grinder: $89.99
- Espresso Tamper: $24.99
- Milk Frother: $29.99

### Merchandise
- BrewCraft Mug: $12.99
- Travel Tumbler: $24.99
- T-Shirt: $19.99
- Tote Bag: $14.99

---

## 🎭 Expected Customer Segments

Your RFM analysis should identify segments similar to these:

### 1. **Champions** (High R, High F, High M)
- Most recent, frequent, and high-value customers
- Strong brand loyalty
- Low churn risk

### 2. **Loyal Customers** (High R, High F, Medium M)
- Regular purchasers with consistent engagement
- Moderate spending
- Good retention potential

### 3. **Potential Loyalists** (Medium R, Medium F, Medium M)
- Showing promise but need nurturing
- Could be upgraded to Loyal segment
- Key target for engagement campaigns

### 4. **At Risk** (Low R, High F, High M)
- Previously valuable customers
- Haven't purchased recently
- High priority for win-back campaigns

### 5. **Hibernating** (Very Low R, Medium F, Low M)
- Long time since last purchase
- Moderate historical engagement
- May respond to reactivation campaigns

### 6. **Lost** (Very Low R, Low F, Low M)
- Very long time since last purchase
- Low historical value
- Lowest priority for retention efforts

### 7. **New Customers** (High R, Low F, Low M)
- Recent first purchase
- Limited purchase history
- Critical for onboarding and retention

---

## 💡 Analysis Tips

### RFM Score Calculation
1. **Recency (R):** Days since last purchase (lower is better)
2. **Frequency (F):** Number of transactions (higher is better)
3. **Monetary (M):** Total amount spent (higher is better)

### Recommended Approach
- Calculate RFM metrics per customer from transaction data
- Use quantile-based scoring (1-5 scale) for each metric
- Combine scores to create RFM segments
- Analyze segment characteristics and behaviors
- Develop targeted marketing strategies

### Advanced Analyses
- Customer Lifetime Value (CLV) calculation
- Churn prediction modeling
- Product affinity analysis by segment
- Channel preference by customer value
- Cohort analysis over time

---

## 📊 Expected Revenue Breakdown

**By Category:**
- Subscriptions: $2,685,982.54 (46%)
- Equipment: $1,558,785.34 (27%)
- Coffee: $1,158,117.92 (20%)
- Merchandise: $439,845.39 (7%)

**By Channel:**
- Website: ~60%
- Mobile App: ~30%
- Retail Partner: ~10%

---

## 🚀 Project Deliverables Checklist

### Analysis Components
- [ ] Data cleaning and validation
- [ ] RFM score calculation
- [ ] Customer segmentation
- [ ] Segment profiling and visualization
- [ ] Revenue analysis by segment
- [ ] Product preference analysis
- [ ] Channel performance analysis

### Visualizations
- [ ] RFM distribution plots
- [ ] Segment size and revenue comparison
- [ ] Customer journey/cohort analysis
- [ ] Product category preferences by segment
- [ ] Time series analysis (trends over 3 years)

### Business Recommendations
- [ ] Targeted marketing strategies per segment
- [ ] Customer retention initiatives
- [ ] Product recommendations
- [ ] Channel optimization suggestions
- [ ] Revenue projection and impact estimates

---

## 🔍 Data Quality Notes

- **No missing values:** Dataset is complete
- **Realistic patterns:** Transaction dates follow realistic customer behaviors
- **Seasonal variation:** Some natural seasonality built into purchase patterns
- **Multi-channel:** Customers may use different channels
- **Repeat purchases:** Customers have varying purchase frequencies

---

## 📝 Citation

**Dataset:** BrewCraft Coffee Subscription (Synthetic)  
**Generated:** January 2026  
**Purpose:** RFM Analysis Portfolio Project  
**Industry:** E-commerce / Subscription Services  

---

**Good luck with your analysis! 🚀☕**
