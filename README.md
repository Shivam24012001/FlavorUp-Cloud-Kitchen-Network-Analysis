# 📦 FlavorUp Order Performance Analysis

## 📘 Project Overview

FlavorUp operates a network of cloud kitchens across Bangalore, leveraging data-driven insights to optimize operations and enhance customer satisfaction. This project analyzes last month's order data to evaluate delivery performance, operational efficiency, and key revenue metrics.

---

## 🎯 Key Objectives

- Analyze order performance by categorizing meal times and tracking peak vs. non-peak orders.
- Assess delivery delays to identify inefficiencies and high-risk locations.
- Conduct a variance sensitivity analysis for different operational stages (processing, packaging, assignment, and delivery).
- Generate actionable insights to enhance the efficiency of FlavorUp’s cloud kitchen operations.

---

## 📁 Dataset Overview

- **Total Orders**: 2,078  
- **Delivered Orders**: 2,030  
- **Cancelled Orders**: 48 (2.31% cancellation rate)  
- **Revenue**: ₹826,053  
- **Revenue Loss due to Stock Out**: ₹31,010  

---

## 🧪 Task 1: Exploratory Data Analysis – Delayed Delivery Analysis

### 🎯 Objective

Evaluate the overall efficiency of the delivery process and present this in a comprehensive dashboard.

### 📌 Delivery Performance Highlights

- **Delayed Deliveries**: 986 (48.57% of total orders)

#### 📅 Weekday vs. Weekend Delayed Rate

| Type     | Peak     | Non-Peak |
|----------|----------|----------|
| Weekday  | 22.05%   | 26.52%   |
| Weekend  | 21.03%   | 27.53%   |

#### 📍 Location-wise Delay Analysis

- Marathahalli: 80.71% delayed  
- Whitefield: 72.68% delayed  
- Jayanagar: 69.86% delayed  

#### 🍽️ Item-wise Delay Due to Preparation Time

- Samosa: 96.67%  
- Noodles: 94.34%  
- Fish Curry: 94.12%  
- Chicken Tikka: 91.11%  
- Ghee Upma: 90.00%  

#### 🚚 Location-wise Delay Due to Delivery Time

- Marathahalli: 83.65%  
- Koramangala: 56.85%  
- Jayanagar: 56.85%  
- Malleswaram: 54.44%  
- BTM Layout: 39.74%  

---

## ⚙️ Task 2: Analysis of Operation Process

### 🎯 Objective

Analyze delays during peak and non-peak periods and conduct a variance sensitivity analysis across different stages.

### 🛠️ Stages in Workflow

- **Preparation**
- **Packaging**
- **Assignment**
- **Delivery**

---

### 📊 Variance Sensitivity Analysis

#### ✅ Interpretation of Variance Table

| Variance Range (%) | Interpretation        |
|--------------------|-----------------------|
| -100% to < -10%    | Way Before Time ⏳    |
| -10% to < 0%       | Before Time 🔵        |
| 0% to < 5%         | On Time ⏱️           |
| 5% to < 40%        | Slight Delay ⚠️      |
| 40% and above      | Delayed 🚨           |
| ≥ 150%             | Immediate Attention ❗ |
| < -60%             | Outlier ❄️            |

---

### 🔍 Stage Categorization Based on Variance

- **Outlier**: Variance < -60%  
- **Immediate Attention**: Variance ≥ 150%  
- Other stages: Based on delay range above

---

### 📝 Prioritization for Overall Remarks (Per Order)

1. **First Priority**: If any stage = *Immediate Attention*, mark the order as **Risk**
2. **Second Priority**: If any stage = *Delayed*, mention as **Delayed**
3. **Third Priority**: If any stage = *Slight Delay*, mention as **Slight Delay**

---

### 🧯 Major Issue Identification Logic

- List all stages with **Immediate Attention** as major issues.
- If none, identify the stage with **maximum variance** among *Delayed* or *Slightly Delayed* stages.

---

## 📦 Task 3: Order Analysis & Dashboard

### 🎯 Objective

Create a dashboard to evaluate order performance and trends.

---

## 📈 Exploratory Data Analysis (EDA)

### 🍽️ Order Time Analysis

| Time    | Orders |
|---------|--------|
| Morning | 525    |
| Noon    | 414    |
| Evening | 503    |
| Night   | 588    |

### ⏰ Peak vs. Non-Peak Orders

- **Peak Time Orders**: 805  
- **Non-Peak Time Orders**: 1,225  

---

## 📊 Order Trends: Peak vs. Non-Peak (by Day)

| Day       | Non-Peak Orders | Peak Time Orders |
|-----------|------------------|------------------|
| Saturday  | 212              | 159              |
| Friday    | 238              | 128              |
| Sunday    | 190              | 119              |
| Thursday  | 160              | 115              |
| Wednesday | 151              | 114              |
| Monday    | 143              | 97               |
| Tuesday   | 131              | 73               |

---

## 💸 Revenue Analysis

### 📦 Average Orders

- **Weekday Orders**: 62  
- **Weekend Orders**: 74.71  

### 💰 Average Revenue

- **Weekday Revenue**: ₹25.2K  
- **Weekend Revenue**: ₹30.3K  

---

## 🔍 Operational Efficiency Summary

### ⚠️ Overall Risk Analysis

- **Total Risk Orders**: 609 (61.76% of total orders)  
  - Preparation Time Delays: 382  
  - Assignment Delays: 159  
  - Delivery Time Delays: 231  

---

## 📊 Dashboard Overview

### 🧰 Tools Used

- **Google Sheets**: Data Cleaning and Calculations  
- **Looker Studio**: Interactive Dashboards and Visualizations  

### 📌 Dashboard Features

- Meal Time and Peak Period Filters  
- Delay Rates by Item and Location  
- Risk and Major Issue Highlight Table  
- Revenue and Order Trends  
- Variance Sensitivity Visualization  

---

## ✅ Final Output

An interactive, dynamic dashboard for management to:

- Identify bottlenecks in operations
- Evaluate high-risk items and locations
- Prioritize stages requiring process improvement
- Monitor order performance and revenue patterns

---

## 📂 Folder Structure

