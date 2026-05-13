# 📊 Adidas Sales Analysis — Power BI Dashboard

> An interactive Power BI dashboard analysing Adidas retail sales performance across regions, products, and retailers in the United States (2020–2021).

---

## 🖼️ Dashboard Preview

![Adidas Sales Dashboard](Adidas_Sales_Dashboard.png)

---

## 📌 Project Overview

This dashboard provides a comprehensive view of Adidas sales data filtered by **Region** and **Invoice Date**. It enables business users to quickly identify top-performing products, retailers, and states, and to monitor key financial KPIs across the Midwest region.

**Data Period:** January 1, 2020 – December 31, 2021  
**Region Filter:** Midwest  
**Tool Used:** Microsoft Power BI Desktop

---

## 🔢 Key Performance Indicators (KPIs)

| KPI | Value |
|-----|-------|
| 💰 Total Sales | **$135.8M** |
| 📈 Operating Profit | **$52.8M** |
| 📦 Units Sold | **391.3K** |
| 🧮 Average Price per Unit | **$40.36** |
| 📊 Operating Margin | **43.5%** |

---

## 📊 Visuals Included

### 1. Total Sales by Month *(Line + Area Chart)*
- Tracks monthly sales from January through December
- Peak sales in **July at $19M**
- Visible dip in **September ($7M)** followed by recovery through December ($17M)

### 2. Total Sales by Region *(Donut Chart)*
- Currently filtered to **Midwest region** = $135.8M (100%)
- Designed to compare multiple regions when filter is removed

### 3. Sum of Total Sales by Product *(Horizontal Bar Chart)*
| Product Category | Sales |
|---|---|
| Men's Street Footwear | $38M |
| Women's Apparel | $28M |
| Men's Athletic Footwear | $21M |
| Men's Apparel | $18M |
| Women's Street Footwear | $16M |

### 4. Total Sales by Retailer *(Horizontal Bar Chart)*
| Retailer | Sales |
|---|---|
| Foot Locker | $48M |
| Sports Direct | $26M |
| West Gear | $23M |
| Kohl's | $22M |
| Amazon | $17M |

### 5. State-Level Sales Table
- Granular breakdown of individual transaction-level sales by **Illinois**
- Ranges from $779 to $1,848 per transaction row
- Useful for drill-down analysis at state level

---

## 🎛️ Filters / Slicers

| Slicer | Description |
|--------|-------------|
| **Region** | Filter by US region (Midwest, West, South, etc.) |
| **Invoice Date** | Date range picker — start and end date |

---

## 📁 Repository Structure

```
adidas-sales-powerbi/
│
├── README.md                        # Project documentation (this file)
├── Adidas_Sales_Dashboard.png       # Dashboard screenshot
├── Adidas_Sales_Analysis.pbix       # Power BI project file
└── data/
    └── adidas_sales_data.xlsx       # Source dataset
```

---

## 🛠️ How to Use

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/adidas-sales-powerbi.git
   ```

2. **Open the `.pbix` file** in [Power BI Desktop](https://powerbi.microsoft.com/desktop)

3. **Refresh the data source** if using your own dataset:
   - Go to `Home → Transform Data → Data Source Settings`
   - Update the file path to your local Excel file

4. **Use the slicers** on the top-right to filter by Region and Invoice Date

---

## 📐 DAX Measures Used

```dax
-- Total Sales
Total Sales = SUM('Sales'[Total Sales])

-- Operating Profit
Operating Profit = SUM('Sales'[Operating Profit])

-- Units Sold
Units Sold = SUM('Sales'[Units Sold])

-- Average Price per Unit
Avg Price per Unit = AVERAGE('Sales'[Price per Unit])

-- Operating Margin
Operating Margin = DIVIDE([Operating Profit], [Total Sales])
```

---

## 💡 Key Insights

- **Foot Locker** is the highest-performing retailer with **$48M** in sales — nearly double Amazon's contribution
- **Men's Street Footwear** is the best-selling product category at **$38M**
- Sales peak mid-year **(July)** and dip sharply in **September**, suggesting a seasonal pattern
- The **operating margin of 43.5%** indicates strong profitability for the Midwest region
- **Women's categories** combined ($28M + $16M = $44M) are competitive with Men's Street Footwear alone

---

## 📋 Requirements

- Microsoft Power BI Desktop (free) — [Download here](https://powerbi.microsoft.com/desktop)
- Windows OS (Power BI Desktop is Windows-only)
- Source data: Excel `.xlsx` format

---

## 👤 Author

**Your Name**  
📧 your.Seelamsudarshanreddy@gmail.com  
🔗 [LinkedIn]([https://linkedin.com/in/your-profile](https://www.linkedin.com/in/sudarshan-reddy-b9ab20256/)) · [GitHub](https://github.com/sudarshan7112/)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).  
Data used is for educational and portfolio purposes only.
