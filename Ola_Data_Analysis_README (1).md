# 🚕 OLA Data Analytics — End-to-End Project

> **Data Analytics project using Excel, SQL and Power BI to analyze ride bookings, revenue, cancellations, vehicle performance and customer/driver ratings.**

![OLA](https://upload.wikimedia.org/wikipedia/commons/1/1c/Ola_Cabs_logo.svg)

## 👨‍💻 Author

**Omkar Bhandalkar**  
Aspiring Data Analyst | SQL | Excel | Power BI | Python

---

## 📌 Project Overview

This project analyzes an OLA-style ride-booking dataset for **Bengaluru** to understand booking performance, ride volume, revenue, cancellations, vehicle types, ride distance and customer/driver ratings.

The project follows an end-to-end analytics workflow:

**Raw Data → Data Understanding → SQL Analysis → Power BI Visualization → Business Insights**

The project package contains the dataset, Power BI report, project brief and supporting dashboard assets.

---

## 🎯 Business Objectives

The analysis focuses on answering questions such as:

- How many bookings were successful?
- What is the booking-status distribution?
- Which vehicle types generate the most ride activity/distance?
- What is the total successful booking value?
- Which payment methods contribute to revenue?
- What are the major cancellation patterns?
- Which customers have the highest booking value?
- How do customer and driver ratings compare?
- What is the average rating across vehicle types?
- How does ride distance vary across the dataset?

---

## 🗂️ Project Structure

```text
Ola_Data_Analysis_end_to_end_Project/
│
├── Bookings.csv
├── OLA Data Analyst Project.pdf
├── Ola_Data_Analysis_end_to_end_Project.pbix
│
└── Ola-Slidesuhub (1)/
    ├── Slide1.PNG
    ├── Slide2.PNG
    ├── Slide3.PNG
    ├── Slide4.PNG
    └── Slide5.PNG
```

### Main Files

| File | Purpose |
|---|---|
| `Bookings.csv` | Source ride-booking dataset |
| `.pbix` | Power BI dashboard/report |
| `OLA Data Analyst Project.pdf` | Project requirements, SQL questions and dashboard requirements |
| `Ola-Slidesuhub (1)` | Supporting dashboard/reference assets |

---

## 📊 Dataset Overview

The current dataset contains:

- **20,407 bookings**
- **20 columns**
- Date range: **1 July 2024 – 30 July 2024**
- 7 vehicle types
- 50 pickup locations
- 50 drop locations
- Multiple booking statuses and payment methods

### Important Columns

| Column | Description |
|---|---|
| `Date` | Booking date |
| `Time` | Booking time |
| `Booking_ID` | Unique booking identifier |
| `Booking_Status` | Booking outcome/status |
| `Customer_ID` | Customer identifier |
| `Vehicle_Type` | Type of vehicle |
| `Pickup_Location` | Ride pickup area |
| `Drop_Location` | Ride destination |
| `V_TAT` | Vehicle time to arrive |
| `C_TAT` | Customer time/arrival metric |
| `Booking_Value` | Booking/fare value |
| `Payment_Method` | Payment method |
| `Ride_Distance` | Distance travelled |
| `Driver_Ratings` | Driver rating |
| `Customer_Rating` | Customer rating |

---

## 🔍 Data Quality Notes

The dataset contains missing values in fields that are naturally dependent on booking outcomes, such as:

- Driver/customer ratings
- Payment method
- V_TAT / C_TAT
- Cancellation details
- Incomplete-ride reason

For example, successful rides contain operational and rating information that may not exist for cancelled bookings.

---

## 📈 Booking Status Analysis

From the supplied dataset:

| Booking Status | Bookings | Share |
|---|---:|---:|
| Success | 12,652 | 62.00% |
| Canceled by Driver | 3,654 | 17.91% |
| Canceled by Customer | 2,081 | 10.20% |
| Driver Not Found | 2,020 | 9.90% |
| **Total** | **20,407** | **100%** |

The successful booking rate is **62%**, matching the target stated in the supplied project brief.

---

## 💰 Revenue Analysis

For successful rides:

**Total successful booking value: ₹6,900,234**

Payment-method breakdown for successful rides:

| Payment Method | Successful Rides | Booking Value |
|---|---:|---:|
| Cash | 6,934 | ₹3,821,738 |
| UPI | 5,113 | ₹2,763,547 |
| Credit Card | 480 | ₹249,494 |
| Debit Card | 125 | ₹65,455 |

---

## 🚗 Vehicle Analysis

The dataset contains these vehicle categories:

- Prime Sedan
- Prime SUV
- Prime Plus
- Mini
- Auto
- Bike
- eBike

The project analyzes vehicle performance using booking volume, ride distance and ratings.

---

## 🧮 SQL Analysis

The supplied project brief defines 10 SQL analysis questions, including:

1. Retrieve all successful bookings.
2. Calculate average ride distance by vehicle type.
3. Count customer-cancelled rides.
4. Find the top 5 customers by number of rides.
5. Count driver cancellations due to personal/car-related issues.
6. Find maximum and minimum driver ratings for Prime Sedan.
7. Retrieve UPI-payment rides.
8. Calculate average customer rating by vehicle type.
9. Calculate total booking value for successful rides.
10. List incomplete rides with their reasons.

These questions are designed to practice filtering, aggregation, grouping, sorting, views and business-oriented SQL analysis.

---

## 📊 Power BI Dashboard

The Power BI report is designed around the major business areas:

### 1. Overall Analysis
- Ride volume over time
- Booking status breakdown

### 2. Vehicle Analysis
- Vehicle-type performance
- Ride distance analysis
- Average customer ratings

### 3. Revenue Analysis
- Revenue by payment method
- Top customers by booking value
- Ride-distance distribution

### 4. Cancellation Analysis
- Customer cancellation reasons
- Driver cancellation reasons
- Cancellation patterns

### 5. Ratings Analysis
- Driver rating distribution
- Customer rating distribution
- Customer vs. driver ratings
- Average ratings by vehicle type

---

## 🛠️ Tools & Technologies

- **Microsoft Excel** — data handling and spreadsheet analysis
- **SQL / MySQL** — querying and business analysis
- **Microsoft Power BI** — interactive dashboards and visualization
- **Python** — part of the broader Data Analyst learning path; Python source code is not included in the current project package

---

## 💡 Key Findings from the Supplied Dataset

- **62%** of bookings were successful.
- **17.91%** were cancelled by drivers.
- **10.20%** were cancelled by customers.
- **9.90%** had the status `Driver Not Found`.
- Successful rides generated **₹6.90M** in booking value.
- **Cash** was the largest successful-ride payment method by booking value in this dataset.
- The dataset contains **20,407 bookings** across **7 vehicle types** and **50 pickup/drop locations**.

---

## ⚠️ Dataset Scope

The supplied project brief describes a larger synthetic dataset generation requirement of **1 lakh rows**, while the dataset included in this project package contains **20,407 rows**.

Therefore, the analysis and numbers in this README are based specifically on the **20,407-row `Bookings.csv` file included with this project**.

---

## 🚀 What I Learned

Through this project, I practiced:

- Understanding a real-world-style business dataset
- Data exploration and data-quality checking
- SQL filtering and aggregation
- `GROUP BY`, `ORDER BY`, aggregate functions and views
- Business KPI analysis
- Power BI dashboard design
- Data visualization
- Converting raw data into business insights
- Presenting an analytics project professionally

---

## 🎓 Project Outcome

This project helped me move from learning individual Data Analytics tools to applying them together in an **end-to-end analytics workflow**.

Instead of only practicing SQL, Excel or Power BI separately, I worked with one business problem and connected the complete process:

```text
Dataset
   ↓
Data Understanding
   ↓
SQL Analysis
   ↓
Business Questions
   ↓
Power BI Visualization
   ↓
Insights & Reporting
```

---

## 📌 Future Improvements

Possible next steps for this project:

- Add a dedicated SQL script file containing all analysis queries
- Add Python/Pandas exploratory analysis
- Add a data-cleaning notebook
- Add DAX measures documentation
- Add more interactive Power BI pages
- Add a project presentation/case-study document
- Publish the Power BI report/screenshots for portfolio use

---

## 📫 Portfolio

**LinkedIn:** Add your LinkedIn profile URL here  
**GitHub:** Add your GitHub repository URL here

---

## ⭐ If You Find This Project Useful

Feel free to explore the project, review the SQL analysis and Power BI dashboard, and share feedback.

**Built as part of my journey toward becoming a Data Analyst.**
