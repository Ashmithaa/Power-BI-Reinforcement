# Car Price Analysis & Prediction using Power BI  

## Project Overview  
The **Car Price Analysis & Prediction** project focuses on analyzing historical automobile data to understand the key factors that influence vehicle pricing. Using **Power BI**, raw data was cleaned, transformed, and visualized into interactive dashboards to uncover meaningful insights.  

This project demonstrates how business intelligence tools can turn raw datasets into **data-driven decisions**.

---

## Objectives  

- Analyze historical car pricing data  
- Clean and transform data using **Power Query Editor**  
- Apply **DAX functions** to calculate KPIs  
- Identify relationships between price and features like brand, fuel type, mileage, and transmission  
- Design an interactive and user-friendly dashboard  
- Generate business insights and recommendations  

---

## Dataset Information  

**Source:** Kaggle – Car Price Prediction Dataset  

**Dataset Features:**
- Brand  
- Model  
- Manufacturing Year  
- Price  
- Mileage  
- Fuel Type (Petrol, Diesel, Electric, Hybrid)  
- Transmission Type (Manual / Automatic)  
- Vehicle Condition (New, Used, Like New)  

~2,000 records  
7 unique car brands  

---

## Data Cleaning & Transformation  

Performed using **Power Query Editor**:

- Removed duplicate records  
- Standardized categorical values  
- Corrected data types  
- Created **Price Category** column (Low / Medium / High)  
- Grouped mileage values  
- Renamed columns for clarity  

---

## DAX Functions Used  

| Function | Purpose |
|---------|---------|
| `SUM()` | Total revenue & mileage |
| `AVERAGE()` | Average price & mileage |
| `COUNT()` | Total number of cars |
| `DISTINCTCOUNT()` | Unique brands |
| `CALCULATE()` | Context-based calculations |
| `IF()` | Price classification |
| `FILTER()` | Conditional logic |
| `ALL()` | Ignore filters |
| `DIVIDE()` | Avoid division errors |
| `YEAR()` | Year trend analysis |

### Sample DAX Measures

```DAX
Total Revenue = SUM('car_price_prediction_'[Price])

Total Cars = COUNT('car_price_prediction_'[Car ID])

Unique Brands = DISTINCTCOUNT('car_price_prediction_'[Brand])

Car Age = YEAR(TODAY()) - 'car_price_prediction_'[Year]

Average Price = AVERAGE('car_price_prediction_'[Price])
```

---

## Dashboard Features  

- KPI Cards (Total Cars, Revenue, Avg Price, Mileage)  
- Brand-wise price comparison  
- Fuel type distribution  
- Vehicle condition analysis  
- Transmission preference  
- Year-wise trends  
- Mileage vs Price analysis  

### Interactivity
- Slicers for Year, Brand, Fuel Type  
- Cross-filtering  
- Dynamic visuals  

---

## Key Insights  

- Premium brands like **BMW** and **Tesla** have higher prices  
- Petrol and Diesel vehicles dominate the market  
- Automatic cars are more preferred  
- New & Like New cars generate higher revenue  
- Electric vehicles show strong price-to-mileage efficiency  

---

## Business Recommendations  

- Focus on premium & automatic vehicles  
- Promote electric vehicles for future demand  
- Use mileage as a key pricing factor  
- Apply data-driven inventory planning  

---

## Conclusion  

This project highlights how **Power BI, DAX, and data visualization** can transform raw automotive data into valuable business insights. It supports smarter decision-making in pricing, sales strategy, and market analysis.

---

## Tools Used  

- Power BI  
- Power Query Editor  
- DAX  
- Data Visualization Techniques  

---

## Author  
**Ashmithaa Pradeep** - Data Analytics & Data Science
