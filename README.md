# Dairy Supply Chain Optimization using Microsoft Fabric
This project uses Microsoft Fabric to build an end-to-end analytics solution for the dairy supply chain. It integrates multi-source data into a unified lakehouse, tracks KPIs like on-time delivery, stock-outs, and return rates, and provides interactive dashboards to identify logistics inefficiencies. By analyzing demand and delivery patterns across products and regions, the solution helps reduce wastage, improve service levels, and optimize supply chain performance — all within Microsoft Fabric.

# 🎯 Objectives
* Reduce stock-outs and lost sales
* Improve delivery performance and operational efficiency
* Minimize product returns and wastage
* Enable data-driven decision-making

# 🛠️ Tools & Technologies
* Microsoft Fabric
* Lakehouse
* Data Warehouse
* Data Pipelines
* Semantic Model
* Power BI
* DAX
* Data Modeling (Fact & Dimension tables)

# 🧱 Complete Microsoft Fabric Workflow
## Step 1: Workspace Creation
* Created a new Fabric workspace named Dairy_Project
* Enabled Lakehouse, Warehouse, and Pipeline capabilities

## Step 2: Data Ingestion into Lakehouse
* Created a new Lakehouse named dairy_lw
* Used Copy Activity to bring data into Fabric Lakehouse and ingest raw data from multiple sources:
    * fact_sales (Fact Table)
    * dim_date (Dimension Table)
    * dim_location (Dimension Table)
    * dim_product (Dimension Table)

## Step 3: Data Warehouse Creation
* Created a Data Warehouse named dairy_dw
* Loaded curated data from Lakehouse into Warehouse using Data Pipelines

## Step 4: Semantic Model Development
* Built a Semantic Model connecting to the Data Warehouse
* Established relationships between fact and dimension tables:
      * fact_sales → dim_product (Product Key)
      * fact_sales → dim_date (Date Key)
      * fact_sales → dim_location (Location Key)

## Step 5: Power BI Dashboard Creation
* Created Power BI Reports within Fabric
* Built interactive dashboards:
      * Dairy Performance Overview – Monitor and optimize dairy business performance
      * Dairy Supply Chain & Inventory Intelligence – Tracks dairy supply, inventory, and distribution performance
      * Returns Analytics & Logistics Efficiency – Reduce wastage and operational inefficiencies
* Added slicers for product category, region, and date range

## Step 6: Publishing & Sharing
* Published dashboards to Fabric workspace

# 📊 Key KPIs Tracked
* On-Time Delivery %
* Return Rate %
* Stock-Out %
* Total Revenue
* Estimated Lost Sales
* Delivery Time

# 📈 Dashboards & Insights

## 1. Dairy Performance Overview
* Monitor and optimize dairy business performance
* View here -

## 2. Dairy Supply Chain & Inventory Intelligence
* Tracks dairy supply, inventory, and distribution performance
* View Here -

## 3. Returns Analytics & Logistics Efficiency
* Reduce wastage and operational inefficiencies
* View here -

# 🧠 Key Business Insights
* Revenue is highly volatile, with sharp dips in February and July despite a peak in May.
* South region consistently outperforms others, contributing the most to the $0.26bn total revenue while returns remain well-controlled below 10%.
* Inventory turnover is very healthy for perishable products, with inventory sold and replaced ~55 times per year.
* Turnover Ratio of 6.67 and (Days Inventory Outstanding) at just one week, indicating efficient stock movement.
* DC-04 shows the highest stock-out risk while DC-08 performs best, leading to an estimated 301K units in lost sales.
* Inventory peaks in August, October, June, and January (with August the highest at 5M units), suggesting potential overstocking or seasonal demand patterns that could be optimized to reduce carrying costs and prevent stock-outs.
* Certain products are overstocked without corresponding sales (driving peak inventory in months like August and January), while other products face stock-outs despite strong demand—contributing to the estimated 301K units in lost sales, particularly at DC-04.
* On-time delivery is critically poor at just 49.3%, yet the return rate remains low at 7.18%
* This suggests that customers are keeping late deliveries because dairy products still have enough remaining shelf life to be usable.
* The South region has a return rate approximately 3x higher than the North and East , indicating a specific logistics or quality issue in that region that requires immediate investigation.
* Returns occur in the same month as sales, confirming they stem from immediate delivery or quality issues (e.g., damage, temperature abuse) rather than delayed shelf-life spoilage — meaning fixing on-time delivery and handling practices could directly reduce losses.
* Total loss due to returns is $19.02M on 225.26K returned units.
* Improving on-time delivery by just 10% would benefit high-volume products like Milk, Curd, Lassi, Butter, and Cheese equally.

# 💼 Business Impact
* This project showcases how Microsoft Fabric can be used to build a scalable, end-to-end analytics solution. It highlights the integration of data engineering and business intelligence to solve real-world supply chain challenges and improve operational efficiency.




