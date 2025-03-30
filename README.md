# FlavorUp Order Performance Analysis

## 📌 Project Overview
FlavorUp operates a network of cloud kitchens across Bangalore, leveraging data-driven insights to optimize operations and enhance customer satisfaction. This project analyzes last month's order data to evaluate delivery performance, operational efficiency, and key revenue metrics.

## 📊 Key Objectives
- Analyze **order performance** by categorizing meal times and tracking peak vs. non-peak orders.
- Assess **delivery delays** to identify inefficiencies and high-risk locations.
- Conduct a **variance sensitivity analysis** for different operational stages (preparation, assignment, and delivery).
- Generate actionable insights to enhance the **efficiency of FlavorUp’s cloud kitchen operations**.

## 📁 Dataset Overview
The dataset includes:
- **Total Orders:** 2,078
- **Delivered Orders:** 2,030
- **Cancelled Orders:** 48 (2.31% cancellation rate)
- **Revenue:** ₹826,053
- **Revenue Loss due to Stock Out:** ₹31,010

## 📈 Exploratory Data Analysis (EDA)
### 📌 Order Time Analysis
- **Meal Time Orders:**
  - Morning: 525
  - Noon: 414
  - Evening: 503
  - Night: 588
- **Peak vs. Non-Peak Orders:**
  - Peak Time Orders: 805
  - Non-Peak Time Orders: 1,225

### 📌 Delivery Performance Analysis
- **Delayed Deliveries:** 986 (48.57% of total orders)
- **Weekday vs. Weekend Delayed Rate:**
  - **Weekday:** Peak (22.05%), Non-Peak (26.52%)
  - **Weekend:** Peak (21.03%), Non-Peak (27.53%)
- **Location-wise Delay Analysis:**
  - Marathahalli: **80.71%** delayed
  - Whitefield: **72.68%** delayed
  - Jayanagar: **69.86%** delayed

### 📌 Item-wise Delay Due to Preparation Time
- Samosa: **96.67%** delayed
- Noodles: **94.34%** delayed
- Fish Curry: **94.12%** delayed
- Chicken Tikka: **91.11%** delayed
- Ghee Upma: **90.00%** delayed

### 📌 Location-wise Delay Due to Delivery Time
- Marathahalli: **83.65%** delayed
- Koramangala: **56.85%** delayed
- Jayanagar: **56.85%** delayed
- Malleswaram: **54.44%** delayed
- BTM Layout: **39.74%** delayed

## ⚙️ Operational Efficiency Analysis
A **Variance Sensitivity Analysis** was conducted for three key operational stages:
1. **Order Preparation** (Primary cause of delays)
2. **Delivery Agent Assignment**
3. **Final Delivery**

Categorization based on variance:
- **Immediate Attention:** Variance ≥ 150%
- **Outliers:** Variance < -60%
- **On Time, Slight Delay, or Delayed:** Based on a defined threshold.

### 📌 Overall Risk Analysis
- **Total Risk Orders:** 609 (61.76% Risk Rate)
  - **Preparation Time Delays:** 382
  - **Assignment Delays:** 159
  - **Delivery Time Delays:** 231

## 📌 Order Trends: Peak vs. Non-Peak
| Order Date | Non-Peak Time Orders | Peak Time Orders |
|------------|---------------------|-----------------|
| Saturday   | 212                 | 159             |
| Friday     | 238                 | 128             |
| Sunday     | 190                 | 119             |
| Thursday   | 160                 | 115             |
| Wednesday  | 151                 | 114             |
| Monday     | 143                 | 97              |
| Tuesday    | 131                 | 73              |

## 📈 Revenue Analysis
### 📌 Average Orders
- **Weekday Orders:** 62
- **Weekend Orders:** 74.71

### 📌 Average Revenue
- **Weekday Revenue:** ₹25.2K
- **Weekend Revenue:** ₹30.3K

## 🚀 Tools Used
- **Google Sheets** - Data Cleaning and Analysis
- **Looker Studio** - Data Visualization

```

## 📢 Future Scope
- Implement **Machine Learning models** for demand forecasting.
