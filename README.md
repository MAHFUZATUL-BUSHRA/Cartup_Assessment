#  <img src="Images/cartup_bangladesh_logo.jpg" width="40"/> Cartup Business Intelligence Case Study
### Business Intelligence Assessment

This project presents a Business Intelligence analysis conducted for Cartup, an e-commerce company that connects customers with sellers while managing warehouse and delivery operations.

The objective of this analysis is to explore operational, commercial, and financial data to identify insights that can improve decision-making across different business teams.

---

# Objectives

• Analyze seller order processing performance  
• Identify operational bottlenecks in the order journey  
• Evaluate rider delivery performance  
• Analyze marketing campaign impact  
• Identify top-performing products and sellers  
• Evaluate financial impact of returns and failed deliveries  

---

# Tools Used

- Power BI
- DAX
- Data Modeling
- GitHub

---

# Dataset Overview

The analysis uses the following datasets:

**dimcustomers** – customer demographics and location  
**dimshops** – seller information  
**dimproducts** – products details  
**dimriders** – delivery rider information  
**campaigndays** – promotional campaign records  
**orderjourneydata** – order lifecycle and operational timestamps

# Data Architecture & Modeling
![P](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/blob/main/Images/Schema.png)
---

# Dashboard Pages

---

# 1️⃣ Order Performance Overview

![Order Performance Dashboard](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/blob/main/Dashboard_Images/Order%20Overview.png)

### Key Metrics

- Total Orders: **125K**
- Delivered Orders: **111K**
- Delivery Success Rate: **89.47%**
- Average Items per Order: **2.08**

### Insights

- Delivery success rate is strong at nearly **90%**, indicating stable logistics performance.
- Order demand is highly concentrated in **Dhaka South, Gazipur, Chattogram, and Sylhet**.
- Male customers contribute **~60% of total orders**, showing higher purchasing activity.

---

# 2️⃣ Seller Order Processing Performance

![Seller Processing Dashboard](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/blob/main/Dashboard_Images/Question%201.png)

### Key Metrics

- Average Seller Processing Time: **50.78 hours**
- Late Processing Rate: **18.44%**
- Fastest Seller Processing: **3.67 hours**
- Slowest Seller Processing: **234.67 hours**

### Insights

- Nearly **1 in 5 orders** are processed later than the expected SLA.
- Some sellers consistently show delayed processing, creating operational delays.
- High-volume sellers may require operational support to handle order loads.

---

# 3️⃣ Order Journey & Operational Bottlenecks

![Order Journey Dashboard](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/blob/main/Dashboard_Images/Question%202.png)

### Insights

- Several operational stages show extended processing times.
- Delays occur in:
  - Pending → RTS
  - RTS → Warehouse
  - Sorting → Last Mile

Hub performance varies significantly.

| Hub | Avg Processing Time | Success Rate |
|----|----|----|
| Warehouse | 50 hrs | 96.84% |
| Tongi Hub | 66 hrs | 88% |
| Agrabad Hub | 41 hrs | 87% |

---

# 4️⃣ Rider Delivery Performance

![Rider Performance Dashboard](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/blob/main/Dashboard_Images/Question%203.png)

### Key Metrics

- Total Riders: **116**
- Total Deliveries: **155K**
- Rider Success Rate: **90.76%**
- Average Delivery Time: **55.41 hours**

### Insights

- Delivery performance varies significantly across riders.
- A small number of riders handle a very large portion of deliveries.
- Some riders show low success rates, indicating training or route issues.

---

# 5️⃣ Campaign Impact on Operations

![Campaign Dashboard](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/blob/main/Dashboard_Images/Question%204.png)

### Key Metrics

- Campaign Days: **24**
- Normal Days: **98**
- Avg Orders per Campaign Day: **2523**
- Avg Orders per Normal Day: **653**
- Order Increase: **286%**

### Insights

- Campaigns drive **nearly 4x higher order volume** compared to regular days.
- Campaign days generate **more than half of total revenue**.
- Sudden order surges may increase pressure on operations.

---

# 6️⃣ Product & Seller Commercial Performance

![Product and Seller Performance Dashboard](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/blob/main/Dashboard_Images/Question%205.png)

### Key Metrics

- Total Revenue: **102.16M**
- Total Profit: **28.69M**
- Average Order Value: **1.93K**
- Total Products: **54K**

### Insights

- FMCG and electronics products generate the highest revenue.
- A small number of products contribute a large share of sales.
- Certain sellers dominate revenue contribution.
- 
![Product Seller Revenue Contribution Dashboard](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/blob/main/Dashboard_Images/Question%205_.png)

### Insights

- The **top 20 sellers** generate a major portion of total platform revenue.
- Sellers such as Shadow Retail and Prime Line Gallery contribute significantly.
- Revenue distribution follows a **Pareto pattern** where few sellers dominate sales.

---

# 7️⃣ Financial Impact of Returns & Delivery Outcomes

![Financial Impact Dashboard](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/blob/main/Dashboard_Images/Question%206.png)

### Key Metrics

- Revenue from Delivered Orders: **130.85M**
- Return Rate: **12.57%**
- QC Rejection Rate: **6.15%**
- Revenue Loss from Failed Deliveries: **16.27M**

### Insights

- Returns and delivery failures create significant financial losses.
- Expected revenue is higher than actual realized revenue.
- Certain product categories show higher return-related losses.

---

# Key Recommendations

### Improve Seller Processing Efficiency
Introduce SLA monitoring and operational support for slow-processing sellers.

### Optimize Operational Pipeline
Address delays in warehouse and sorting stages.

### Improve Rider Performance
Implement route optimization and rider training programs.

### Prepare for Campaign Surges
Increase operational capacity during promotional campaigns.

### Strengthen Commercial Strategy
Focus marketing on top-performing sellers and high-demand products.

### Reduce Revenue Loss
Improve quality checks and delivery verification processes.

---

---

# Dashboard Files

You can explore the dashboard using the following files:

📊 **Power BI Dashboard (PBIX)**  
[Download PBIX File](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/tree/main/Dashboard)

📄 **Dashboard Presentation (PDF)**  
[View Dashboard PDF](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/blob/main/Dashboard_PDF.pdf)


---

# Key Takeaways

This analysis provided several important insights about Cartup’s operations and business performance:

• Order demand is highly concentrated in major urban areas such as **Dhaka South and Gazipur**.

• Seller processing efficiency varies significantly, with **18% of orders processed later than the expected SLA**.

• Promotional campaigns significantly increase demand, generating **nearly 4x higher order volumes** compared to regular days.

• A small number of sellers and products contribute to a large portion of **total revenue**, indicating a strong **Pareto distribution**.

• Returns and failed deliveries lead to **substantial revenue losses**, highlighting the need for improved delivery success and quality control processes.

---

# Conclusion

This Business Intelligence analysis demonstrates how operational and transactional data can be leveraged to uncover meaningful insights in an e-commerce business.

By analyzing the order lifecycle, seller performance, delivery operations, and marketing campaigns, the dashboard identifies key opportunities to:

- Improve seller processing efficiency  
- Optimize warehouse and delivery operations  
- Prepare operational capacity for marketing campaigns  
- Strengthen commercial strategy around high-performing products and sellers  
- Reduce financial losses caused by returns and delivery failures  

These insights can support Cartup in improving operational performance, enhancing customer satisfaction, and increasing overall profitability.

---

# Author

**Mahfuzatul Bushra Tisha**  
Data Analyst | Aspiring AI Engineer

📍 Bangladesh  


---

⭐⭐⭐ 
