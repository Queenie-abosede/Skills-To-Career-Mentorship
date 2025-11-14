# Telecoms Customer Churn Analysis
## Table of Content
1. [Introduction](#💡-introduction)  
2. [Project Overview](#project-overview)
3. [Business Question](#business-question)
4. [Methodological Approach](#methodological-approach)
5. [Tools Used](#tools-used)
6. [Data cleaning and transformation](#data-cleaning-and-transformation)
7. [Data analysis and Visualization](#data-analysis-and-visualization)
9. [Key Insights](#key-insights)
10. [Recommendation](#recommendation)
11. [Limitation](#limitation)
12. [Conclusion](#conclusion)
13. [File Included](#file-included)
14. [Author](#author)

## 💡 Introduction
We are a telecommunication company that provides phone and internet services to thousands of people across California, but every month, a significant number decide to leave us for a competitor or simply cancel their service. Our company is bleeding customers, and we don't fully understand why. This "customer churn" is more than just a number, it's lost revenue, wasted marketing expenses, and a sign that we might not be meeting our customers' needs.

The core problem is that we lack clarity. We have all this customer data, but we haven't connected the dots to see the story telling us about who is leaving, when they leave, and most importantly, why, which is why we need a customer insight Analyst.


## 📘 Project Overview
The telecommunication company is experiencing customer turnover (churn), which affects revenue stability and growth. However, the reasons behind customer churn are unclear. There’s a need to identify patterns, trends, and key factors influencing churn to guide retention strategies.

The project was executed in Microsoft Excel, featuring two interactive dashboards:
1. Churn Customer Demographics –  detailed breakdowns Customer demographics
2. Customer Churn Analysis – Identofy the trends, patterns and key factors Influenecing Churn


## 🎯 Business Question
1. Is our service portfolio failing us? Which specific service (e.g., Fiber Optic internet, online security, streaming) is most strongly associated with customers leaving?
2. What is the gender distribution of churned customers?
3. What is our exact customer churn rate?
4. Do specific payment methods or billing structures correlate with higher churn rates?
5. What are the common demographics (like age, gender, Marital status) and contract characteristics (month-to-month vs. yearly) of customers who churn?
6. Does tenure contribute to churn rate?


## 🧰 Methodological Approach
The analysis merges customer behavioral data with zip code demographic information to identify patterns across multiple dimensions. Initial focus includes descriptive analytics to establish baseline metrics, followed by correlation analysis to identify key churn drivers. The final deliverables will provide prioritized recommendations based on both statistical significance and business impact.
The primary tool utilized for data inspection, integrity checking, and cleaning was Microsoft Excel, specifically leveraging its advanced Power Query and filtering features.

## 🧰 Tools Used
Tool	Purpose
1. Microsoft Excel	Data cleaning, analysis, and dashboard creation
2. Pivot Tables	Summarizing large datasets
3. Slicers	Enabling interactive filtering by Customer Status
4. Charts & Graphs	Visual representation of trends and Patterns

## Data Cleaning and transformation
-	Categorical Inputation (Non-Churned Customers): Null entries within the Churn Category were replaced with “Customers” since their status was *stayed and joined* which means they are still existing customers, and Churn Reason columns were replaced with the descriptive value *"N/A"*. This decision reflects the business logic that an empty value in these specific fields signifies the customer is still active. Some null values were found in other services columns that were replaced with *"unverified"* because they were a boolean response of *"yes or no"*.
-	Numerical Imputation (Zero Replacement): Null values in quantitative fields, such as *Avg Monthly GB Download*, were replaced with 0.
-	Created calculated fields: Generated churn flags, tenure segments, and revenue categories.
-	Geographic Validation: Standardized city names and ensured proper coordination with the zip code database.


## 📈 Data Analysis and Visualization
1. **KPIs:**
-	Overall churn rate (26.54%)
-	Geographic performance across 1,106 cities
-	Revenue impact by customer segment ($3.68M churn revenue)

  
2. **Trends and Pattern:**
-	Customer demographics (gender, marital, age and dependancy ratio)

  <img width="1106" height="549" alt="image" src="https://github.com/user-attachments/assets/dd5b55e8-6bee-46ce-a250-8d1f2401bb5e" />

  

-	Service performance by type (Fiber Optic, DSL, Cable)

  <img width="591" height="433" alt="image" src="https://github.com/user-attachments/assets/b1432f1c-9372-4962-b98f-81909f419ac5" />

  

-	Contract type analysis (month-to-month vs. term contracts)

  <img width="576" height="428" alt="image" src="https://github.com/user-attachments/assets/9ad537d4-b4ba-456c-9df1-a020a58580f3" />

  

-	Payment method correlation with churn

<img width="625" height="432" alt="image" src="https://github.com/user-attachments/assets/092ba062-09c2-4f75-ab26-789165bf0bb7" />


 
-	Offer made availabe to Customers with churn

  <img width="586" height="412" alt="image" src="https://github.com/user-attachments/assets/ce3e9599-add1-4f15-aebf-b2440184ad0b" />

  

-	Reasons why Customer Churned

  <img width="624" height="409" alt="image" src="https://github.com/user-attachments/assets/763bd538-aad9-45b8-b3f3-31a6927d813e" />




## 📊 Key Insights 
• **Insight:** Churn is heavily concentrated among month-to-month contract customers (1,655 churners) and those using Fiber Optic internet (70%), indicating dissatisfaction with commitment flexibility and service quality. Customers without online backup and without offers also have significantly higher churn rates. The age range 39–58 shows the highest churn volume, suggesting mid-life customers may have stronger expectations for reliability and pricing.

• **Insight:** A major driver of churn is service dissatisfaction, as seen in the high churn from categories like competitor switching, dissatisfaction, and attitude issues. The absence of online backup and high churn among Fiber Optic customers may signal gaps in technical support responsiveness. Customers with dependents are churn-prone, showing that households may need more reliable and responsive support.

• **Insight:** Churned customers represent a significant revenue loss given the average total charge of $1,531 and the high volume of churn across key segments. The dominance of Fiber Optic churn suggests that high-value customers are leaving. The churn rate of 26.5% impacts long-term cash flow predictability, particularly due to month-to-month contracts.

• **Insight:** The high churn among Fiber Optic users (70%) signals dissatisfaction with performance or reliability, despite it being a premium service. Many customers on basic or no-offer plans are leaving, suggesting unmet expectations in value packaging. Month-to-month contract churn indicates that commitment models may need redesigning.
 
• **Insight:** The organization faces a 26.5% churn rate, with the majority of losses coming from high-value, Fiber Optic customers and month-to-month contracts. This churn is disproportionately driven by dissatisfaction, competitive pressure, and service experience gaps. Churn is highest in prime economic age groups (39–58), which hold significant revenue-generating potential.

       

## 🔍 Recommendations
1. Head of Marking Head should Prioritize a targeted retention campaign for month-to-month customers—offer price incentives, loyalty bonuses, or flexible upgrade plans. Improve perceived value for Fiber Optic users through speed boosts or reduced downtime. Launch personalized retention offers for adults age 38–58, focusing on stability, value, and service assurance.
2. Customer Service Team should Strengthen your first-contact resolution rate and ensure faster escalation for Fiber Optic complaints. Implement a follow-up system for customers who call more than once within 30 days. Train agents on empathy and proactive retention techniques to address “attitude” as a churn reason.
3. Finance Head Team Model the financial impact of reducing churn by 5–10% within the high-value Fiber Optic segment to justify budget for retention campaigns. Re-assess pricing strategy for month-to-month customers, offering bundles that increase retention without significantly affecting ARPU. Allocate funds to improve service reliability, as this directly influences revenue retention.
4. Product and Service Team should prioritize quality improvements in the Fiber Optic offering—speed consistency, uptime, and installation experience. Redesign product bundles to include online backup, offers, or loyalty benefits to increase value perception. Review and enhance the month-to-month contract experience with flexible but attractive upgrade paths.
5. CEO/Executive Management should adopt a company-wide churn reduction strategy that aligns marketing, customer service, product, and technical teams. Invest in service reliability enhancements, especially for Fiber Optic customers. Set quarterly churn-reduction KPIs and prioritize retention as a top-level strategic initiative to protect revenue and competitive positioning.


## Limitation
Analyzing population impact was difficult due to the "one-to-many" relationship between cities and zip codes, preventing clean data aggregation.

## 📜 Conclusion
The company should prioritize reducing churn by improving Fiber Optic service quality and reliability, as it’s the main driver of revenue loss. The CEO and executives should lead a cross-departmental effort in Marketing to retain month-to-month Fiber users through targeted offers, Customer Service to enhance Fiber installation and support, Product Team should improve service performance and bundle add-ons for retention, and Finance to fund these initiatives. This coordinated action will strengthen customer loyalty, reduce revenue churn, and protect long-term profitability.

        
## 📂 Files Included
File Description:
[https://drive.google.com/drive/folders/1lyJ5bBK2THVo_pi7M9K4RhHXs_0o-fgS?usp=sharing]


## 🧑‍💻 Author

Esther Adewumi
Data Analyst | Business Analyst | Researcher
📧 [estheradewumi829@gmail.com]




