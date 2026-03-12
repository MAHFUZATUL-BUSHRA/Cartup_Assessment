#  <img src="Images/cartup_bangladesh_logo.jpg" width="40"/> Cartup Business Intelligence Case Study
### Business Intelligence Assessment

This Case Study presents a Business Intelligence analysis conducted for Cartup, an e-commerce company that connects customers with sellers while managing warehouse and delivery operations.



---

# Objectives
The objective of this analysis is to explore operational, commercial, and financial data to identify insights that can improve decision-making across different business teams.

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
- Order demand is highly concentrated in **Dhaka, Gazipur, Chattogram, and Sylhet**, highlighting key urban markets.
- Male customers contribute **~60%** of total orders, showing higher purchasing activity.
- A small group of top customers places disproportionately more orders, emphasizing the importance of customer retention.
- Order volume spikes in **November–December**, suggesting seasonal demand or promotional opportunities.
- Several states show low order activity, presenting opportunities for geographic expansion and targeted marketing.
---

# 2️⃣ Seller Order Processing Performance

![Seller Processing Dashboard](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/blob/main/Dashboard_Images/Question%201.png)

### Key Metrics

- Average Seller Processing Time: **50.78 hours**
- Late Processing Rate: **18.44%**
- Fastest Seller Processing: **3.67 hours**
- Slowest Seller Processing: **234.67 hours(~9.7 days)**
- Late Seller Rate: **58.19%**

### Insights

- Nearly **1 in 5 orders** are processed later than the expected SLA(Considered 48hrs).
- A majority of shops (1,882 vs 1,352) process orders late,suggesting systemic operational issues rather than isolated cases.
- Some sellers (10+) consistently show extreme delays (7–9 days), significantly affecting overall platform performance.
- High-volume sellers do not necessarily process orders slower; low-volume sellers often contribute disproportionately to delays.
- Efficient processing practices exist: some sellers manage high order volumes with extremely low late rates, indicating operational best practices can be replicated.

---

# 3️⃣ Order Journey & Operational Bottlenecks

![Order Journey Dashboard](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/blob/main/Dashboard_Images/Question%202.png)

### Insights

- Rider Assignment is the Major Bottleneck:Rider assignment to delivery stage takes  **~55.41 hours**, contributing the largest share of total delivery time.
- Mid-Pipeline Stages Cause Noticeable Delays:Pending → **RTS (~20.08 hrs) and RTS → FM (~16.61 hrs)** highlight internal operational inefficiencies.
- Sorting and Hub Operations Are Efficient:Delays from **Sorting → Last Mile (~5.55 hrs) and FM → Sorting (~2.55 hrs)** are minor, indicating well-functioning warehouse operations.
- Regional Delivery Performance Varies:Urban hubs like Dhaka North/South show high success **(~92%)** and shorter delivery times, while other regions experience longer delays.
- Certain Source Hubs Contribute to Delays:CB Hub **(~133 hrs)** and some 3PL hubs **(~113 hrs)** significantly slow down processing, whereas hubs like Uttara/Jatrabari are more efficient.
- Order Pipeline Drop Indicates Operational Failures:**~10%** of orders do not reach delivery due to cancellations or operational issues, showing room for improvement in fulfillment reliability.**• Total Orders: 124,515 • Sorted Orders: 123,300 • Last Mile Orders: 123,300 • Delivered Orders: 111,400**

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
- Total Deliveries(Packages): **155K**
- Rider Success Rate(Package): **90.76%**
- Average Deliveries per Rider: **960.34**
- Failed Deliveries: **~14K**
- Average Delivery Time: **55.41 hours**

### Insights

- Delivery performance varies significantly across individual riders, highlighting inconsistencies in last-mile operations.
- A small group of riders handles a disproportionately large number of deliveries, suggesting uneven workload distribution and potential operational risk.
- Some riders demonstrate low delivery success rates (~79–86%), indicating potential challenges in routes, operational inefficiencies, or performance issues.
- Top-performing riders achieve very low average delivery times (~5–6 hours), showing that faster last-mile delivery is achievable with optimized routing.
- Geographic factors influence performance, as delivery activity is concentrated in major regions (e.g., Dhaka), while less-dense areas may face slower deliveries.
- Performance segmentation identifies clear groups of Average and Low Performers, providing targeted opportunities for training and operational improvement.
- Operational inefficiencies, such as 14K failed deliveries and high average delivery time, indicate that workload management and route optimization could further improve overall delivery efficiency.
- Rider success and speed are not always correlated—some riders achieve high success rates but take longer per delivery, highlighting potential for efficiency gains through process standardization.

---

# 5️⃣ Campaign Impact on Operations

![Campaign Dashboard](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/blob/main/Dashboard_Images/Question%204.png)

### Key Metrics

- Campaign Days: **24**
- Normal Days: **98**
- Avg Orders per Campaign Day: **2523**
- Avg Orders per Normal Day: **653**
- Order Increase: **286%**
- Campaign Revenue Share: **52.2%**
- Delivery Success Rate (Campaign Days): **93.23%**
- Delivery Success Rate (Normal Days): **85.90%**
- Average Rider Delivery Time (Campaign Days): **52.6 hrs**
- Average Rider Delivery Time (Normal Days): **58.33 hrs**

### Insights

- Campaigns drive **~4x higher order volume** than normal days.
- Campaign days contribute **>50% of total revenue** despite being only **~20%** of days.
- Delivery success rate is higher during campaigns **(93.23% vs 85.9%)**, showing effective planning.
- Average rider delivery time is **~6** hours faster on campaign days.
- Major campaigns **(e.g., Big November Hunt)** create short-term demand spikes, stressing operations.
- Higher discounts directly increase order volume, but may reduce margins.
- Sorting stage shows potential bottlenecks during peak campaign periods.
- Campaigns increase overall profitability despite heavy discounts **(14.99M vs 13.7M)**.

---

# 6️⃣ Product & Seller Commercial Performance

![Product and Seller Performance Dashboard](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/blob/main/Dashboard_Images/Question%205.png)

### Key Metrics

- Total Revenue: **102.16M**
- Total Profit: **28.69M**
- Average Order Value: **1.93K**
- Total Products: **54K**
- Top Seller Revenue Share: **20.67%**
- Top Product RevenueShare: **1.71%**

![Product Seller Revenue Contribution Dashboard](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/blob/main/Dashboard_Images/Question%205_.png)

### Insights

- FMCG and Electronics dominate revenue: FMCG drives high order volume; electronics deliver high revenue per order.
- Revenue concentrated among few sellers: Top sellers contribute >20% of total revenue, highlighting platform dependence.
- Urban markets lead performance: Dhaka, Gazipur, Chattogram, and Narayanganj generate most revenue.
- Household essentials drive demand: Top products include oil, milk powder, rice, and detergents.
- High-cost products yield strong profit: Investment in high-demand categories like FMCG and electronics delivers strong ROI.
- Product portfolio is large but skewed: 54K products attract diverse customers, but revenue is driven by a small subset.
- Operational efficiency supports commercial success: High delivery success rates (~90%+) from top sellers reinforce reliable performance.
- Category-wise strategy matters: FMCG = high volume; Electronics = high value; Fashion & Lifestyle = moderate/niche demand.
- Investment in high-demand product categories results in strong profit returns.
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
- Revenue Loss from Returned Orders: **3.50M**
- Revenue Loss from Rejected Orders (QC): **239.37K**
- Revenue Loss Due to Order Failures: **20.01M (~13.27% of potential revenue)**

### Insights

- Failed Deliveries Drive Most Financial Losses:**81% of revenue loss (~16.27M)** comes from failed deliveries, highlighting operational inefficiencies in last-mile logistics.
- Returns Are a Significant Contributor:A return rate of **12.57%** indicates challenges with product quality, fit, or misalignment between product descriptions and customer expectations. Fashion and Lifestyle categories are most impacted.
- QC Rejections Affect Operational Efficiency:**6.15%** of products fail pre-shipment quality checks, leading to inventory inefficiencies and additional handling costs.
- Failed deliveries are the largest contributor to revenue leakage.
- Fashion and Lifestyle categories experience higher return-related losses.
- High-Risk Products and Sellers Identified:Certain **products (e.g., Luminous Robust Durability Wardrobe, Leather Jacket Winter Proof)** and **sellers (e.g., Elite Square Shop, Alpha Center Shop)** disproportionately contribute to revenue leakage due to returns, delivery failures, or quality issues.
- Regional Disparities:Revenue losses are concentrated in specific areas **(Savar 44.40%, Keraniganj 36.28%, Narayanganj 32.81%)**, suggesting logistics challenges or delivery inefficiencies in these regions.
- Revenue Gap Analysis:Expected revenue (~150M) vs. realized revenue (130.85M) indicates nearly 20M in unrealized revenue, meaning over 1 in 8 potential revenue Taka is lost due to operational inefficiencies.
- Operational & Strategic Implications:Improving delivery success, reducing returns, monitoring high-risk sellers, and optimizing logistics in high-loss regions could recover significant revenue (~5–6M if failed deliveries are reduced by 30%) and improve overall profitability.

---

# Dashboard Files

You can explore the dashboard using the following files:

📊 **Power BI Dashboard (PBIX)**  
[Download PBIX File](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/tree/main/Dashboard)

📄 **Dashboard Presentation (PDF)**  
[View Dashboard PDF](https://github.com/MAHFUZATUL-BUSHRA/Cartup_Assessment/blob/main/Dashboard_PDF.pdf)

---
# Interpretation of Findings

### Cartup’s operational, commercial, and financial data reveal several key patterns affecting performance:

#### 1. Operational Efficiency

* Seller processing is slower than expected: the average processing time is 50.78 hours, more than double the 24-hour SLA.
* Nearly 1 in 5 orders are delayed, and over half of sellers consistently exceed SLA, indicating systemic inefficiencies.
* Operational bottlenecks primarily occur during early order stages (Order → Pending, Pending → RTS) and last-mile delivery (Rider Assignment → Delivery, ~55 hours), while warehouse and sorting operations are relatively efficient.
* Rider performance is inconsistent, with a small subset handling disproportionately high volumes and some showing low delivery success rates (~79–86%).

#### 2. Commercial Performance

* Revenue and orders are concentrated in a few top-performing sellers and urban markets (Dhaka, Gazipur, Chattogram, Narayanganj), creating dependence on select sellers and regions.
* FMCG and Electronics dominate platform revenue, with household essentials driving high volume and electronics delivering high order value.
* Campaigns significantly boost order volumes (~286% higher than normal days) and revenue (~52% contribution), while operational teams maintain or slightly improve delivery performance during peak periods.

#### 3. Financial Impact

* Operational inefficiencies result in a revenue loss of ~13.27% of potential revenue (~20.01M), primarily due to failed deliveries (~81% of losses) and returns (12.57% return rate).
* Fashion and Lifestyle products contribute disproportionately to revenue loss, driven by returns and QC rejections.
* Regional disparities exist: Savar, Keraniganj and Narayanganj show exceptionally high revenue loss rates (44.40%, 36.28% and 32.81%, respectively), highlighting logistics and last-mile delivery challenges.

#### Overall Implications for Cartup

* While core operations and campaigns perform reasonably well, systemic delays, seller inefficiencies, and last-mile issues reduce customer satisfaction and financial performance.
* High dependence on top sellers, high-volume products, and select urban markets creates commercial risk.
* Targeted interventions in seller operations, last-mile logistics, product quality, and campaign planning can recover significant revenue and improve operational reliability.

---
# Key Recommendations

### 1.Improve Seller Processing Efficiency
##### Introduce SLA monitoring and operational support for slow-processing sellers.
* Enforce a 24-hour SLA and monitor compliance via automated alerts and dashboards.
* Conduct operational audits and training for slow-processing sellers (e.g., Summit Corner House, Silver Base Retail, Global Base Retail).
* Share best practices from top-performing sellers to improve workflow consistency.
* Introduce incentives (badges, priority listing, or financial rewards) for consistent SLA adherence.

### 2.Optimize Operational Pipeline
##### Address delays in warehouse and sorting stages.
* Streamline early-stage order processing (Order → Pending → RTS) with automation and real-time readiness notifications.
* Implement hub-specific operational improvements for high-delay hubs (CB Hub, select 3PL hubs).
* Use predictive staffing and resource allocation during peak seasons or campaigns to prevent bottlenecks.

### 3.Improve Rider Performance
##### Implement route optimization and rider training programs.
* Balance rider workload distribution to prevent over-reliance on a few top performers.
* Provide training and route optimization tools for low-performing riders.
* Monitor KPIs (success rate, failed deliveries, delivery time) and incentivize high performance.
* Expand local rider fleets in regions with longer delivery times.
  
### 4.Prepare for Campaign Surges
##### Increase operational capacity during promotional campaigns.
* Focus on high-impact campaigns (e.g., Big November Hunt) with dedicated operational and marketing support.
* Use predictive analytics to forecast demand and allocate resources efficiently.
* Balance discount strategy with margin preservation to ensure campaign profitability

### 5.Strengthen Commercial Strategy
##### Focus marketing on top-performing sellers and high-demand products.
* Reduce dependence on top sellers by onboarding and incentivizing mid-tier sellers.
* Promote high-revenue categories (Electronics, FMCG) with targeted campaigns and cross-selling strategies.
* Focus marketing and logistical support on urban hubs with the highest demand and revenue potential.
* Expand geographic coverage in low-activity regions to capture new markets.

### 6.Reduce Revenue Loss
##### Improve quality checks and delivery verification processes.
* Target failed deliveries with address verification, delivery confirmations, and route optimization.
* Minimize returns in high-loss categories (Fashion, Lifestyle) via improved product listings, sizing guidance, and accurate descriptions.
* Monitor high-risk products and sellers using performance scorecards (returns, QC failures, delivery success).
* Optimize logistics in high-loss regions with reliable partners and localized fulfillment solutions.

---

---

# Conclusion

Cartup demonstrates strong commercial and operational performance in core urban markets and high-demand categories. However, operational inefficiencies, uneven seller and rider performance, high returns, and regional logistics challenges reduce profitability and customer satisfaction. Strategic improvements across seller management, last-mile delivery, high-risk products, and campaigns can recover revenue, enhance operational efficiency, and support sustainable platform growth.
These insights can support Cartup in improving operational performance, enhancing customer satisfaction, and increasing overall profitability.

---

# Author

**Mahfuzatul Bushra Tisha**  
Data Analyst | Aspiring AI Engineer

📍 Bangladesh  


---

⭐⭐⭐ 
