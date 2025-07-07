# RDAMP-Sales-Analysis

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
  i. Portable Solar Generator  
  ii. Portable Refrigerator Freezer  
  iii. Electric Bike  
  iv. Compact Dishwasher  
  v. Digital Camera

### 3. Bottom 5 Underperforming Products  
Bottom 5 Products are:  
  i. Cinnamon Raisin Bagels (GBP 2.73)  
  ii. Canned Black Beans  
  iii. Baking Soda  
  iv. Paprika  
  v. Instant Mashed Potatoes (GBP 4.19)

### 4. Highest Margins by Product Category  
Top Categories by Margin:  
  i. Food - Dressing (79%)  
  ii. Food - Salad Toppings (71%)  
  iii. Food - Cereal (69%)  
  iv. Food – Breakfast Foods (69%)  
  v. Grooming (69%)

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

![image](https://github.com/user-attachments/assets/42d3a9e2-bb71-46c9-9c89-6a3f9361085b)
