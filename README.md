# CodeAlpha_Sentiment-Analysis
# Hotel Booking Analytics Dashboard

## Data Cleaning & Reporting Automation using Power BI

---

# Project Overview
This project automates data cleaning and reporting workflows using Power BI. The dashboard analyzes hotel booking data and provides insights into bookings, revenue, cancellations, and customer behavior through interactive visualizations.

---

# Tools Used
- Power BI
- Power Query
- DAX

---

# Dataset
Dataset Used: `hotel_bookings.csv`

The dataset contains:
- Hotel details
- Customer information
- Booking dates
- Revenue data
- Cancellation status

---

# Data Cleaning Process
- Removed duplicate records
- Handled missing values
- Corrected data types
- Standardized text values
- Removed unnecessary columns
- Created calculated columns and measures

---

# DAX Measures

## Total Bookings
```DAX
Total Bookings =
COUNTROWS(hotel_bookings)
```

## Average ADR
```DAX
Average ADR =
AVERAGE(hotel_bookings[adr])
```

## Cancellation Rate
```DAX
Cancellation Rate =
DIVIDE(
    COUNTROWS(
        FILTER(
            hotel_bookings,
            hotel_bookings[is_canceled] = 1
        )
    ),
    COUNTROWS(hotel_bookings)
) * 100
```

---

# Dashboard Features
- KPI Cards
- Monthly Booking Trends
- Revenue Analysis
- Cancellation Analysis
- Customer Segmentation
- Country-wise Analysis
- Interactive Slicers

---

# Slicers Used
- Hotel Type
- Year
- Month
- Country
- Customer Type
- Booking Status

---

# Key Insights
- Seasonal booking trends were identified
- Cancellation rates differ across hotel types
- Revenue varies by month and customer segment
- Customer distribution changes by country

---

# Outcome
This project improved understanding of:
- Data Cleaning
- Reporting Automation
- Dashboard Development
- KPI Analysis
- Business Intelligence using Power BI

---

# Conclusion
The Hotel Booking Analytics Dashboard successfully automates data cleaning and reporting processes using Power BI and provides interactive business insights through professional visualizations.
