<p align="center">
  <img src="banner.png" alt="Nescafe Sales Data Analysis Banner" width="100%">
</p>

<h1 align="center">☕ Nescafe Sales Data Analysis Project</h1>

<p align="center">
  <b>Tool Used:</b> Google Sheets &nbsp; | &nbsp;
  <b>Level:</b> Spreadsheet Data Analysis Practice &nbsp; | &nbsp;
  <b>Scope:</b> Section A – Section E
</p>

---

## 📌 Project Overview

This project analyzes the **Nescafe Sales Dataset**, which contains product, sales, marketing, and customer information across multiple markets.

### 🎯 Objectives

- Perform structured data cleaning  
- Apply spreadsheet text and date functions  
- Conduct logical validation checks  
- Perform business aggregation analysis  
- Compare budget vs actual performance  

All tasks were completed using **Google Sheets functions and Pivot Tables**.

---

# 🧹 Section A – Data Cleaning & Text Functions

### 1️⃣ Check Blank Promo Codes
```excel
=IF(AN2="","Missing","Available")
```

### 2️⃣ Remove Non-Printable Characters (Customer Name)
```excel
=CLEAN(V2)
```

### 3️⃣ Remove Extra Spaces
```excel
=TRIM(V2)
```

### 4️⃣ Replace Spaces with Hyphen
```excel
=SUBSTITUTE(V2," ","-")
```

### 5️⃣ Count Characters in Product Name
```excel
=LEN(E2)
```

### 6️⃣ Convert Customer Name to Proper Case
```excel
=PROPER(V2)
```

### 7️⃣ Convert City to Uppercase
```excel
=UPPER(AJ2)
```

### 8️⃣ Convert City to Lowercase
```excel
=LOWER(AJ2)
```

---

# 📅 Section B – Date & Time Functions

### 1️⃣ Format Order Date
`Format → Custom Date → DD-MMM-YYYY`

### 2️⃣ Display Today’s Date
```excel
=TODAY()
```

### 3️⃣ Display Current Date & Time
```excel
=NOW()
```

### 4️⃣ Extract Year
```excel
=YEAR(T2)
```

### 5️⃣ Extract Month
```excel
=MONTH(T2)
```

### 6️⃣ Extract Day
```excel
=DAY(T2)
```

### 7️⃣ Extract Day Name
```excel
=TEXT(T2,"dddd")
```

### 8️⃣ Calculate Days Since Order
```excel
=TODAY()-T2
```

### 9️⃣ Find Month End Date
```excel
=EOMONTH(T2,0)
```

---

# 🔄 Section C – Data Transformation & Combination

### 1️⃣ Combine Product Line & Product
```excel
=F2 & " - " & E2
```

### 2️⃣ Combine City, State, Market
```excel
=AJ2 & ", " & J2 & ", " & C2
```

### 3️⃣ Create Full Location Field
```excel
=AJ2 & ", " & J2 & " (" & C2 & " Market)"
```

---

# ✅ Section D – Logical Checks

### 1️⃣ Identify Missing Promo Codes
```excel
=IF(AN2="","Missing","Available")
```

### 2️⃣ Count Promo Code = SAVE10
```excel
=COUNTIF(AN:AN,"SAVE10")
```

### 3️⃣ Count Blank Promo Codes
```excel
=COUNTIF(AN:AN,"")
```

---

# 📊 Section E – Aggregation & Business Analysis

### 1️⃣ Total Sales for Coffee
```excel
=SUMIF(I:I,"Coffee",U:U)
```

### 2️⃣ Average Profit for Central Market
```excel
=AVERAGEIF(C:C,"Central",T:T)
```

### 3️⃣ Count Sales Records per Market
```excel
=COUNTIF(C:C,"Central")
```

Also analyzed using **Pivot Tables** for complete market comparison.

### 4️⃣ Sales Variance (Actual vs Budget)
```excel
=U2 - M2
```

### 5️⃣ Identify Negative Profit (Loss)
```excel
=IF(T2<0,"Loss","Profit")
```

---

# 📈 Key Skills Demonstrated

- Data cleaning & preprocessing  
- Text transformation functions  
- Date extraction & time calculations  
- Conditional logic handling  
- Business KPI aggregation  
- Budget vs Actual comparison  
- Pivot table analysis  

---

# 🏁 Project Completion Status

| Section | Status |
|----------|--------|
| Section A – Data Cleaning | ✔ Completed |
| Section B – Date Functions | ✔ Completed |
| Section C – Data Transformation | ✔ Completed |
| Section D – Logical Checks | ✔ Completed |
| Section E – Aggregation & Analysis | ✔ Completed |

Section F (Business Insights) can be added as an advanced extension.

---

# 📂 How to Use

1. Open the dataset in Google Sheets.  
2. Apply formulas exactly as structured above.  
3. Use Pivot Tables for aggregated reporting.  
4. Analyze performance gaps and profitability trends.  

---

## 👤 Author  
**Data Analysis Practice Project – Spreadsheet Analytics**
