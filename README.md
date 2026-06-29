# [Power BI] Financial_Analysis

## 📑 Table of Contents
1. [📌 Overview](#-overview)  
2. [📂 Dataset & Data Model](#-dataset--data-model)  
3. [🧠 Design Thinking Process](#-design-thinking-process)  
4. [📊 Key Insights & Visualizations](#-key-insights--visualizations)  
5. [🔎 Final Conclusion & Recommendations](#-final-conclusion--recommendations)

---

## 📌 Overview

### Project Overview
This project focuses on analyzing corporate financial data for the fiscal year 2023 using Power BI. By building an interactive financial dashboard, it provides a comprehensive visualization of the company's financial health, cost structure, and operational efficiency.

### Problem Statement
* **Track Profitability Flow:** Clearly map out the exact journey from Gross Revenue down to the final Net Profit.
* **Analyze Cost Structures:** Identify which specific expense categories and subgroups are consuming the largest portions of the budget.
* **Evaluate Performance:** Compare the financial efficiency of different business lines over time to support strategic and operational decisions.

### Core Business Questions
To solve this problem, the dashboard was designed to answer three critical financial questions:
1. **The Profit Bridge:** What is the exact path from Gross Revenue down to Net Profit, and which major expense categories (COGS vs. Opex) are putting the most pressure on our margins?
2. **Segment Profitability:** Among our core business lines (Sportswear, Sports Equipment, and Nutrition), which are the true "cash cows" driving profit, and which are operating at a loss?
3. **Operational Efficiency:** How do our total expenses trend month-over-month compared to revenue growth, and where can we optimize costs?

---

## 📂 Dataset & Data Model
The dataset (`Financial_analysis_dataset.xlsx`) contains the core financial data:
* **`revenue_expense`:** Raw transaction-level data including Date, Amount, Category (Revenue/Expense), Subgroup, and Business Line.
* **`dictionary`:** A reference sheet explaining the definitions and hierarchies of the financial categories used in the dataset.

### Data Model
This project utilizes a **Star Schema** architecture to ensure performance and analytical flexibility in Power BI. One main Fact table tracks all financial transactions (revenue and expenses). This connects to shared Dimension tables for dates (`Calendar`), categories (`Dim_category`, `Dim_SubGroup`), and business units (`Dim_Business_line`).

<img width="976" height="567" alt="Data Model" src="https://github.com/user-attachments/assets/172d5f08-81c5-4017-a661-b277d1f8ea64" />

---

## 🧠 Design Thinking Process
To ensure this dashboard delivers real business value rather than just displaying raw numbers, I applied a structured Design Thinking approach. This helped bridge the gap between technical data modeling and the actual needs of the business stakeholders (CFOs & Finance Managers).

### 1️⃣ Empathize (5W1H Problem Statement)
<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/d7d20a10-c2cf-494f-a853-0ccb9a18a6e5" />


### 2️⃣ Define Point of View (POV)
<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/56ba9645-1c62-45c0-b2b2-46bf5b5a9ef5" />


---

## 📊 Key Insights & Visualizations  

### 🔍 Dashboard Preview  

#### 1️⃣ Dashboard 1: Financial Overview Preview  
<img width="1159" height="625" alt="image" src="https://github.com/user-attachments/assets/3e44a648-8c69-479e-99c4-b4989d7aa41f" />

* **Observation:** The company demonstrates strong performance with Total Revenue reaching $17.6M and a Net Profit Margin of 24.6%. However, the Revenue to Net Profit Bridge (Waterfall chart) shows that revenue is heavily consumed by COGS (~$7M) and Opex (~$6M). **Additionally, the overview immediately flags the "Nutrition" segment as the only division operating at a loss, dragging down the overall profitability.**
* **Recommendation:** Since COGS and Opex account for over 69% of total revenue, the operations team must audit internal inefficiencies. **Immediate attention is also required to investigate the root causes of the "Nutrition" division's negative performance.**

#### 2️⃣ Dashboard 2: Business Line Analysis Preview 
<img width="1157" height="622" alt="image" src="https://github.com/user-attachments/assets/9d6fe07c-4480-4699-b3b1-642c9fb5f288" />


* **Observation:** Diving deeper into segment performance, while "Sports Equipment" generates high revenue volume, the true profit engine is "Sportswear", delivering an impressive $2.74M in Net Profit. Conversely, the "Nutrition" segment is confirmed to be bleeding cash with a -$0.71M loss.
* **Recommendation:** Conduct an immediate financial audit into the "Nutrition" division's cost structure. If the -$0.71M loss cannot be reversed through aggressive cost-cutting, leadership should consider pausing this segment. Simultaneously, reallocate capital to scale the highly efficient "Sportswear" division.

#### 3️⃣ Dashboard 3: Cost Structure Analysis Preview  
<img width="1148" height="608" alt="image" src="https://github.com/user-attachments/assets/eeff6cd8-e43a-4f33-8387-4a098c55ade9" />


* **Observation:** A detailed breakdown of the cost structure explicitly shows that **Labor** is the largest expense subgroup, vastly outweighing other operational costs and constantly pressuring the margins across all divisions.
* **Recommendation:** Implement stricter budget caps and monthly tracking mechanisms specifically focusing on Labor costs to prevent budget overruns.

---

## 🔎 Final Conclusion & Recommendations

📌 **Key Takeaways:**
* **Heavy Cost Burden:** Top-line revenue is strong ($17.6M), but operational costs (COGS and Opex) consume over 69% of it. The company maintains a 24.6% profit margin, but it is heavily pressured by these expenses.
* **Winner vs. Loser Segment:** The "Sportswear" division is the ultimate profit engine ($2.74M Net Profit), while the "Nutrition" segment is actively bleeding cash (-$0.71M loss).
* **Top Expense Driver:** The cost structure analysis proves that Labor is the highest operational expense.

🚀 **Key Actions:**
* **Stop the Bleed:** Conduct a thorough financial audit on the "Nutrition" division. If costs cannot be optimized, pause this segment to protect the total company profit.
* **Focus on Stars:** Reallocate capital and strategic focus toward the highly efficient "Sportswear" line to maximize the overall Return on Investment.
* **Control Key Costs:** Implement strict monthly budget caps and ROI tracking specifically for Labor to prevent further margin erosion.
