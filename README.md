# Supplier-Quality-and-Performance-Dashboard

<img width="639" alt="Screenshot 2024-11-05 220245" src="https://github.com/user-attachments/assets/b8b1b682-b1cc-45d9-a27c-2c7e8aee93d0">

## Overview
The Supplier Quality and Performance Dashboard provides a comprehensive view of supplier performance, focusing on defect quantity, downtime, and their impacts on overall operations. 
This analysis reveals key insights into vendor, plant, and material performance, helping stakeholders make data-driven decisions.

**Problem Statement:**

The manufacturer currently lacks a procurement system and consistent standards to evaluate supplier quality across plants, resulting in difficulties in identifying which suppliers deliver quality goods and which cause production issues. 
The management team has gathered data on materials, defects, vendors, defective material counts, and downtime minutes caused by defects from multiple plants. They seek assistance to visualize, analyze, and draw insights from this data to address key questions:

1. Which vendors or plants have the highest defect counts?
2. Which vendors or plants are responsible for the most downtime?
3. Are there specific material-vendor combinations that perform poorly?
4. Are there specific vendor-plant combinations that perform poorly?
5. How does performance vary across different plants for the same vendor and material?
The business also hopes for additional insights that may have been overlooked, and they want the analysis to leverage Power BI.

The dataset includes the following columns:

1. Date - Date of entry or incident.
2. Vendor - Name of the supplier or vendor.
3. Plant Location - Location of the supplier plant.
4. Category - Type of product supplied.
5. Material Type - Specific type of material.
6. Defect Type - Classification of the defect's impact (e.g., "No Impact", "Rejected").
7. Defect - Specific defect type (e.g., "Bad Bearings", "Not Certified").
8. Total Defect Qty - Quantity of defective materials.
9. Total Downtime Minutes - Duration of downtime attributed to each defect.

<img width="877" alt="Supplier" src="https://github.com/user-attachments/assets/6c30673e-b6ff-419c-88e5-29b198de642e">

## Analysis and visualization steps:
**Normalization of Dataset**
Normalization is important for efficient data processing, especially in large databases or applications. 
It reduces data inconsistencies, makes databases easier to scale and update, and optimizes performance for queries and reporting.
The main table was splited into into six dimension tables; Vendor, Plant, Category, Material Type, Defect Type and Defect using power bi

**Modelling**
After normalizing the data set and creating a date table, the data set was modeled using a star schema model to link our dimension tables, date table and fact table together

 
<img width="928" alt="Screenshot 2024-11-05 214602" src="https://github.com/user-attachments/assets/4bc5a938-e870-47de-a042-0846a3d0eedb">

## Performance Breakdown

### Vendor Performance:

Vendors like Yombu, Avamm, and Meejo have the highest defect quantities, with Yombu topping the list at approximately 15 million defects.
Vendor risk levels are categorized into high, medium, and low. High-risk vendors demonstrate a higher defect quantity, posing a significant impact on production efficiency.

### Plant Location Performance:

Top Defective Plants: Hingham, Charles City, and Twin Rocks are the top three locations with high defect quantities. Hingham leads with over 100 million reported defects.
Impact Analysis: Defects at these plants lead to substantial downtimes, with Westside, Weaverville, and Waldoboro having notable downtime hours due to defective products.

### Defect Type:

Common defect categories include Not Certified and Bad Seams, contributing heavily to downtime hours.
Defects such as “Not Certified” have the highest downtime impact, with 13.8K hours lost.
Material Performance:

Raw Materials and Corrugate materials contribute significantly to downtime hours, each incurring over 50K downtime hours.
Materials

**for a comprehensive view of the analysis, here is the link to my interactive dashboard**: [Click Link](https://app.powerbi.com/view?r=eyJrIjoiZGFhMmYwZWQtNmQwOC00MGIyLThjNjYtYmE0YTdlOGFhMmJlIiwidCI6ImZjZmYwYzY1LTQwMTMtNDFhZS04Mjc2LTExNDZiZDA4ZDY5OSIsImMiOjh9)


## General Recommendations
### To reduce downtime and enhance overall performance, manufacturing firms can consider the following recommendations:

**Implement Preventive Maintenance**: Routine maintenance schedules for machines and equipment can prevent unexpected breakdowns, reducing downtime and ensuring reliable operation.

**Strengthen Supplier Quality Control**: Regularly audit and evaluate suppliers to ensure consistent quality and timeliness of raw materials. 
Setting performance benchmarks and penalties for non-compliance can also motivate suppliers to maintain quality standards.

**Invest in Training Programs**: Train staff on machine handling, maintenance best practices, and quality control. 
Skilled employees are more likely to identify and resolve issues quickly, reducing the potential for downtime.

**Adopt Data-Driven Decision-Making**: Utilize dashboards and analytical tools, like Power BI, to continuously monitor defect rates, downtime hours, and cost impacts. 
Data-driven insights enable informed decision-making and faster response times to operational issues.

**Optimize Inventory Management**: Avoid shortages of essential materials by implementing an inventory management system that aligns with production schedules. 
This reduces downtime caused by material unavailability.

**Foster Collaboration with Vendors and Plants**: Establish strong communication channels with high-risk vendors and underperforming plants to collaboratively solve issues, improve performance, and reduce defect rates.

Through a proactive approach to downtime management, manufacturing firms can achieve higher operational stability, improve quality, and enhance their competitiveness in the market.


