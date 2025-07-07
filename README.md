# RDAMP Sales Analysis

## A) Data Cleaning & Preparation

### 1. Uploaded CSV File & Saved as Excel  
- Downloaded the raw `.csv` dataset.  
- Converted it into `.xlsx` format to enable advanced calculations in Excel.

### 2. Incorrect Region, City, and Country  
- Verified **Region**, **City**, and **Country** using the **Store Locations Dataset**.  
- Used `VLOOKUP` based on the common **Postal Code** field to correct mismatches and omissions.  
- Incorrect entries were **highlighted in red** for visibility.

### 3. Negative Sales and Cost Price  
- Negative values were identified as **returns** or **data errors**.  
- All rows with **negative sales or cost price** were removed to ensure accurate reporting of business performance.

### 4. Missing Categories  
- Sub-categories were used to infer missing categories using **Python mapping** techniques.  
- Entries without a matching category were excluded for accuracy.

### 5. New Aggregated Columns Created  
The following calculated fields were added to the dataset:
- `Discounted Price`: Final price after applying discount.
- `Total Sales (Excluding Discount)`: Original sales amount.
- `Total Sales (Including Discount)`: Sales after applying discount.
- `Total Cost Price`: Total cost incurred.
- `Total Revenue`: Actual earnings from sales post-discount.
- `Profit Margin`: `(Revenue - Cost) / Revenue * 100`

---

## B) Exploratory Data Analysis (EDA) & Visualization

### 1. Sales Distribution across Order Mode  
- A **Pie Chart** was created to show the proportion of **Online vs In-Store** sales.

### 2. Top 5 Best-Selling Products  
1. Portable Solar Generator  
2. Portable Refrigerator Freezer  
3. Electric Bike  
4. Compact Dishwasher  
5. Digital Camera

### 3. Bottom 5 Underperforming Products  
1. Cinnamon Raisin Bagels (£2.73)  
2. Canned Black Beans  
3. Baking Soda  
4. Paprika  
5. Instant Mashed Potatoes (£4.19)

### 4. Highest Margins by Product Category  
Top 5 Categories by Profit Margin:
1. Food - Dressing (79%)  
2. Food - Salad Toppings (71%)  
3. Food - Cereal (69%)  
4. Food – Breakfast Foods (69%)  
5. Grooming (69%)

### 5. Top 5 Profitable Regions  
1. East Midlands (England)  
2. Scotland  
3. London (England)  
4. Yorkshire & The Humber (England)  
5. Southwest England

### 6. Revenue Comparison  
- A **Line Chart** illustrates monthly profit trends by year.  
- **May 2024** had the highest monthly revenue.  
- **2025** shows a consistent **upward trend** in both revenue and profitability compared to 2024.

---

## C) Dashboard

An interactive dashboard was created summarizing key metrics including:
- Sales performance  
- Profit margin analysis  
- Regional profitability  
- Product-wise performance  
- Year-over-year revenue trends
