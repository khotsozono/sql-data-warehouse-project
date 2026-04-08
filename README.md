## Hi, I'm Khotso Zono

🎓 Information Science Graduate | 📊 Junior Business Intelligence Developer | 📈 Aspiring Data Analyst

This project marks the beginning of my journey in Business Intelligence and data analytics, and it is the first of many projects I plan to develop as I continue growing in this field. I am committed to continuously learning, improving my technical and analytical skills, and staying adaptable to new tools and technologies. My goal is to use data-driven insights to help organizations make informed decisions, improve efficiency, and ultimately become more profitable through the value created by my work.

---

## SQL Data Warehouse Project

 This project involved designing and building a SQL-based data warehouse from scratch using the Medallion Architecture approach. The solution was structured into bronze, silver, and gold layers to support efficient data ingestion, transformation, and analytics-ready reporting. Through this project, I applied data modeling and SQL transformation techniques to organize and refine raw data into meaningful business information. The development process was completed with guidance and learning resources from Data with Baraa, who helped strengthen my understanding of modern data warehousing practices. 

 This project involves:

* **Data Architecture**: Designing a Modern Data Warehouse Using Medallion Architecture Bronze, Silver, and Gold layers.
* **ETL Pipelines**: Extracting, transforming, and loading data from source systems into the warehouse.
* **Data Modeling**: Developing fact and dimension tables optimized for analytical queries.

---

## Data Architecture 

The data architecture for this project follows Medallion Architecture: **Bronze**, **Silver**, and **Gold** layers: 


<p align="center"> 
 <img width="800" height="500" alt="Data Warehouse Architecture (1)" src="https://github.com/user-attachments/assets/29d8582f-9cef-4ee0-b8e0-eb3163db3c76" />

* **Bronze Layer**: Stores raw data as-is from the source systems. Data is ingested from CSV Files into SQL Server Database.  

* **Silver Layer**: This layer includes data cleansing, standardization, and normalization processes to prepare data for analysis.
  
- **Gold Layer**: Houses business-ready data modeled into a star schema required for reporting and analytics.


--- 

## Data Flow   

 The data flow of this SQL data warehouse follows the Medallion Architecture, moving data through Bronze, Silver, and Gold layers to progressively improve data quality and usability. Raw data from CRM and ERP source systems is first ingested into the Bronze layer, where it is stored in its original form for traceability. The data is then cleaned, standardized, and integrated in the Silver layer, ensuring consistency and readiness for analysis. Finally, the refined data is transformed into business-focused models in the Gold layer, where fact and dimension tables (such as sales, customers, and products) are created to support reporting, analytics, and decision-making. 
 
<p align="center"> 
<img width="700" height="500" alt="Data Flow Diagram" src="https://github.com/user-attachments/assets/880779ab-2de9-42a8-b24b-d1c93d44714a" />

--- 
## Data Integration 

The data integration layer combines information from both CRM and ERP systems to create a unified view of customers, products, and sales activity. The CRM system provides transactional sales data through **crm_sales_details**, which links customer information (**crm_cust_info**) and product information (**crm_prd_info**) using shared keys. The ERP system enriches this data by adding additional customer and product context, including customer location details from **erp_loc_a101**, extended customer attributes from **erp_cust_az12**, and product category information from **erp_px_cat_g1v2**. By connecting these tables through common identifiers such as customer IDs, product keys, and category IDs, the integration process consolidates operational and transactional data into a consistent structure that supports accurate analytics and reporting within the data warehouse.

<p align="center"> 
<img width="750" height="650" alt="Data Intergration Visual" src="https://github.com/user-attachments/assets/edaaf3c7-fad4-4964-9cc0-08c8956ceb71" />

 --- 

 ## Sales Data Mart (Gold Layer)  

The Sales Data Mart forms part of the Gold layer of the data warehouse and is designed using a star schema to support fast and efficient reporting. At the center of the model is the fact table (gold.fact_sales), which stores measurable business events such as orders, sales amounts, quantities, prices, and important dates related to each transaction.

The fact table connects to two dimension tables, gold.dim_customers and gold.dim_product: which provide descriptive context for the sales data. The **dim_customers** table contains customer-related attributes such as name, gender, country, and demographic information, while the **dim_product** table stores product details including product name, category, subcategory, and product line.

The relationships between the tables follow a many-to-one structure. Each record in the fact table represents a single sales transaction and includes foreign keys (customer_key and product_key) that link back to the dimension tables. This means that many sales records in the fact table can relate to one customer in the customer dimension and one product in the product dimension.
 <p align="center"> 
 <img width="670" height="427" alt="Star Schema Data Model drawio" src="https://github.com/user-attachments/assets/43d55b52-8306-43a0-a0c4-275ca2e90a41" />

---  

Through this project, I strengthened my practical skills in SQL, data modeling, and data transformation while gaining a deeper understanding of how data warehouses support business intelligence and decision-making. As my first data warehouse project, it represents a strong foundation for future work, and I look forward to continuing to expand my knowledge and building more advanced data solutions that help organizations make smarter, data-driven decisions. 

---

## 📬 Connect With Me

* LinkedIn: www.linkedin.com/in/khotso-zono-671491301
* Email: khotsozono@gmail.com


---
 
 Open to graduate programmes, junior BI roles, and data analytics opportunities.
