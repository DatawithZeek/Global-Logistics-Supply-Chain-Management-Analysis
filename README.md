# Global-Logistics-Supply-Chain-Management-Analysis
Global Chain Performance &amp; Cost Optimization Improving Delivery Reliability, Reducing Cost &amp; Controlling Logistics Cost 

<img width="656" height="374" alt="global chain 1" src="https://github.com/user-attachments/assets/3986eba6-ffb8-490a-bca2-6a4f154ce0f0" /> 

# Project Overview 
This project focuses on analyzing global logistics and supply chain operations using Power BI, SQL, and DAX to identify operational inefficiencies, improving delivery performance, optimize inventory management, and control logistics costs.

The analysis explores suppliers reliability, transportation performance, inventory availability, product quality, and supply chain disruptions to provide actionable insights that support data-driven decision-making. 

The project aims to help the company reduce late deliveries, short deliveries, and stockouts while keeping freight and inventory holding costs under control.

# Business Problem
The company faces challenges in maintaining reliable deliveries and sufficient inventory while managing operational cossts.

Key business challengies include:
- Late deliveries affecting supply chain reliability
- Short deliveries resulting in incomplete order fulfillment
- Stockouts disrupting inventory availability
- High freight costs across carrier and transportation lanes
- Inventory holding costs assoiciated with excess stock
- Product defects and rejected quantities affecting supply chain efficency
- Supplier and transportation disruptions impacting delivery performance

# Business Objectives 
 
# How can the company reduce late deliveries, short deliveries, and stockouts while keeping freight and inventory holding costs under control ?

The analysis aims to identify the root causes of supply chain inefficiencies and recommend practical strategies for improving operational performance 

# Project Objectives 
  1. Evaluate suppliers and carrier delivery performance
  2. Identify factors contributing to late and short deliveries
  3. Analyze stockout patterns across products and warehouses
  4. Investigate freight costs across transportation lanes and carriers
  5. Assess product quality using rejected quantities and defect rates
  6. Examine the relationship between delivery delays and inventory shortages
  7. Identify opportunities to improve supply chain efficiency and cost management
  8. Provide actionable recommendations for management

# # Data Description 

The datasets consists of 11 interconnected tables representing different aspects of global logistics and supply chain operations

| Table            |           Description |
|---|---|
dim_carriers      |    Contains carrier information used to analyze transportation performance 
dim_date          |    Date dimension used for time-based analysis and reporting 
dim_lane          |    Contains transportation lane information for route- level analysis 
dim_products      |    Contains product information for product- level analysis 
dim_suppliers     |    Contains supplier information for suppliers performance analysis 
dim_warehouses    |    C0ntains warehouse information for inventory and operational analysis 
fact_inventory_monthly| Contains monthly inventory records and stockout indicators 
fact_purchase_orders | Contains purchase order information used to analyze procurement and replenishment
fact_shipments    |    Contains shipment information, delivery performance, transit time, freight costs, and quality- related metrics 
ref_disruotion_events  | Contains supply chain disruption information for investigating operational interuptions
ref_market_indicatior  | Contains market-related indicators that may provide context for supply chain performance 

# Tool & Technology 
| Tool |Purpose |
|---|---|
Power Query | Data cleaning and transformation 
Power BI    | Data modelling, visualization, and dashboard development 
DAX         | KPI calculations and analytical measures
GitHub      | Project documentation and portfolio presentation 

# Data Cleaning & Preparation 

Data preparation was an important stage of the project to ensure consistency, accuracy, and reliability before analysis.

The cleaning process focused on the following areas:

1. Data Inspection
   - Reviewed the structure of all 11 tables
   - Identify relevant columns for delivery, inventory, procurement, and cost analysis
   - Examine data types and fields formats
   - Identified key fields required for relationships between tables
2. Data Type Validation
   - Verified date fields were stored using appropriate date formats
   - Checked numerical fields such as quantities, freight costs, and transit days
   - Ensured identifier fields such as suppliers IDs, product IDs, and shipment IDs were treated as catergorical identifiers rather than measures
3. Missing Value Assessment
   - Identified missing values in relevant analytical fields
   - Evaluate missing records should be retained / flagged
   - Avoided replacing missing values with arbitrary figures that could distort the analysis
4. Duplicate Record Assessment
   - Checked for duplicate records in fact and dimension tables
   - Reviewed potential duplicate shipment, purchase order, and inventory observations
   - Ensured aggregation methods reflected the appropriate level of detail in each table
5. Data Consistency
   - Validated binary indicator fields such as on_time_flag, in_full_flag, otif_flag, and stockout_flag
   - Reviewed consistency between delivery quantities and rejected quantities
   - Investigated the existing defect rate percentage against quantity-based calculations
 6. Data Modeling
   - Organized the dataset using a dimensional model
   - Connected fact tables to relevant dimension tables using appropriate keys
   - Used the date dimension to support time-based analysis

 # # Key Performance Indicators (KPIs)

     The following KPIs were developed to measure supply chain performance
     
     KPI | Description |
     |---|---|
     On-Time Delivery Rate | Percentage of shipments delivered on time
     OTIF Rate  | Percentage of shipments delivered both on time and in full
     Late Deliveries | Number of shipments that failed to arrive on time
     Short Deliveries | Number of shipments that were not delivered in full
     Stockout Rate | Percentage of inventory observations marked as stockout
     Freight Cost | Total transportation expenditure recorded in the shipment data
     Holding Cost | Inventory holding expenditure, where supported by the dataset
     Average Lead Time Days | Average actual transit time in days
     Defect Rate | proportion of delivered quantity rejected due to quality issues

# Analysis & Business Questions 

The analysis was guided by the following business questions:

  1. What percentage of shipments are delivered on time?
  2. How many deliveries are short, and what is the short delivery rate?
  3. What is the company's overall OTIF performance?
  4. Which products and warehouses experience the most stockouts?
  5. Which suppliers have the poorest delivery performance?
  6. Which carrier and transportation lanes have the highest freight costs?
  7. How can inventory holding costs be balanced against stockout risk?
  8. Which products and suppliers have the highest defect rates?
  9. Are transportation delays associated with stockouts?
  10. Which transportation lanes provide the best balance between cost and delivery reliability?

# Key Findings 

 1. Delivery Performance
  - Overall On-Time Delivery Rate **86.10%**
  - Overall OTIF Rate **80.98%**
  - **SUP-100326 & SUP-101400** are with the lowest OTIF performance of **20%**each 
  - **CAR-031** is the with the highest late delivery frequency of **1812** 
    
2. Short Deliveries
  - Total short deliveries **5K**
  - Short Deliveries rate **5.91%**
  - **Apparel** is the highest short deliveries of **984** 

3. Inventory & Stockouts
  - Overall Stockout Rate **11.61%**
  - **WH-EWR-01 848** is the highest stockout frequency 
  - **Apparel** is most frequently affected by stockouts 

4. Logistics Costs
  - Total Freight Cost **$1.53BN**
  - **Air** is the highest freight cost
  - **CAR-014** Is the highest freight cost per unit of **4.52**

5. Product Quality
  - Overall Defect Rate **1.59%**
  - Total Rejected Quantity **$19.5M**
  - **SUP-100971** with the highest rejection rate
    
     
      



