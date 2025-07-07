# RDAMP-Sales-Analysis
## Project Overview  
This project focuses on analyzing sales data for RDAMP to identify high-performing products, underperformers, and profitability trends across different regions and categories. 
The goal is to clean the data, extract meaningful insights, and build an interactive dashboard for business decision-making.

---

## A) Data Cleaning for Analysis

### 1. Uploaded CSV File & Saved as Excel  
- Downloaded the raw csv dataset and converted it into .xlsx file for advanced calculations.

### 2. Incorrect Region, City and Country  
- The Region, City and Country were checked from the Store Locations Dataset ensure the data is consistent.
- There were omissions as well as incorrect assignments detected which was resolved using VLOOKUP from Store Location Dataset with the help of the Postal Code (Common Value in both sheets).  
- The incorrect rows are highlighted with red colour.

### 3. Negative Sales and Cost Price  
- Negative sales or cost prices usually happen because of errors or returns. These values don’t show real sales or costs and can confuse the analysis.  
- To keep the data clean and accurate, all rows with negative sales or costs are removed so the report shows true business performance.

### 4. Missing Categories  
- Many products or sub-categories were repeated in the data with consistent categories. Python was used this to fill in missing categories by mapping each sub-category to its known category.
- The entries for which no category was found were excluded from the database to keep the results accurate.

### 5. New Aggregated Columns Created  
Fields added to the dataset for further analysis:
- **Discounted Price**: The final price after applying the discount to the original sale price.
- **Total Sales (Excluding Discount)**: Original sales amount before discount.
- **Total Sales (Including Discount)**: Actual sales amount after discount is applied.
- **Total Cost Price**: The total amount it cost to acquire or produce the items.
- **Total Revenue**: The actual income earned from sales after applying discounts.
- **Profit Margin**: The percentage of revenue that remains as profit after deducting costs.

---

## B) EDA & Visualization

### 1. Sales Distribution across Order Mode  
- Created a Pie Chart to understand the ratio in which sales occur (Online Vs In-Store)

### 2. Top 5 Best-Selling Products  
  The Top 5 Products are:  
  1. Portable Solar Generator  
  2. Portable Refrigerator Freezer  
  3. Electric Bike  
  4. Compact Dishwasher  
  5. Digital Camera

### 3. Bottom 5 Underperforming Products  
  Bottom 5 Products are:  
  1. Cinnamon Raisin Bagels (GBP 2.73)  
  2. Canned Black Beans  
  3. Baking Soda  
  4. Paprika  
  5. Instant Mashed Potatoes (GBP 4.19)

### 4. Highest Margins by Product Category  
  Top Categories by Margin:  
  1. Food - Dressing (79%)  
  2. Food - Salad Toppings (71%)  
  3. Food - Cereal (69%)  
  4. Food – Breakfast Foods (69%)  
  5. Grooming (69%)

### 5. Top 5 Profitable Regions  
  The Regions are:  
  1. East Midlands (England)  
  2. Scotland  
  3. London (England)  
  4. Yorkshire & The Humber (England)  
  5. Southwest England

### 6. Revenue Comparison  
- The Line chart shows different lines indicating each year and the profit earned in each month.
- May 2024 shows highest revenue earned in a month, while the 2025 revenue has an upward trend and better profits than 2024.

---

## C) Dashboard  
Interactive Power BI Dashboard was created to summarize and visualize the key metrics from the analysis.  
It includes:
- Sales Distribution Model Revenue Proportions  
- Profit Margin by Category  
- Year-over-year revenue comparisons (Monthly Trends) 
- Profitable Regions
- Top and Bottom 5 Products by Revenue

![image](https://github.com/user-attachments/assets/42d3a9e2-bb71-46c9-9c89-6a3f9361085b)

---

## D) Recommendations

1. **Optimize Inventory for Best-Selling Products**  
   Maintain adequate stock levels and promotional activities for top-selling products such as *Portable Solar Generators*, *Electric Bikes*, and *Compact Dishwashers* to maximize revenue.

2. **Prioritize High-Margin Product Categories**  
   - Focus on expanding and promoting products in *Food - Dressing (79%)*, *Salad Toppings (71%)*, and *Cereal/Breakfast Foods (69%)*, as they offer the highest profit margins.  
   - Consider bundling these products or offering volume discounts to further boost sales while preserving high profitability.

3. **Enhance Omnichannel Strategy**  
   While in-store sales slightly lead (51.55%), online sales are close behind (48.45%).  
   Consider strategies to:  
   - Increase cross-channel marketing.  
   - Offer loyalty rewards or click-and-collect models to merge physical and digital channels.

4. **Intensify Regional Marketing in High-Performing Areas**  
   Focus expansion and targeted marketing in top-performing regions such as *East Midlands*, *Scotland*, and *London*.

5. **Leverage Seasonal Sales Peaks**  
   Schedule key promotions and product launches in *May* to capitalize on historically high monthly revenue.

6. **Scale Operations Based on 2025 Growth Trends**  
   Invest in operations, logistics, and digital infrastructure to support the strong upward revenue momentum seen in *March 2025*.

----

## Tools & Technologies  
- Excel for initial data cleaning and transformation.
- Python (pandas, numpy) for automation and data preparation. 
- Power BI Dashboard for interactive visualization. 
- VLOOKUP for location correction

## File Descriptions

| File Name                               | Description                                                                                       |
|----------------------------------------|----------------------------------------------------------------------------------------------------|
| Ace Superstore Retail Dataset(in).csv  | Raw sales data containing transactions, product details, and sales figures.                        |
| Karunesh_Sehgal_Cleaned_dataset.xlsx   | Cleaned and processed sales dataset saved in Excel format, with added aggregated columns.          |
| Karunesh_Sehgal_Data_Cleaning.ipynb    | Python Jupyter notebook used for data cleaning, including filling missing categories and handling inconsistencies. |
| Karunesh_Sehgal_Sales_Dashboard.pbix   | Interactive dashboard presenting key visualizations and insights derived from the analyzed sales data. |
| README.md                              | Documentation file for the project.                                                                 |
| Store Locations(Store Locations).csv    | Dataset mapping postal codes to accurate regions, cities, and countries for location validation.    |
