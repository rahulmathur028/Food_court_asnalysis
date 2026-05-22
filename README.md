# 🍔 Swiggy Food Court & Restaurant Performance Analytics

## 📌 Project Overview
This project presents a comprehensive **Food Delivery Analytics Dashboard** focused on restaurant performance, sales distributions, and consumer ordering behaviors across a major food aggregator network (Swiggy ecosystem). By structuring unstructured culinary data, the repository delivers clear operational insights regarding geographic revenue hubs, timing bottlenecks, and product type margins.

## 📊 Key Insights & Analytics Covered
The project processes granular order receipts to establish critical business milestones:

* **Executive Performance KPIs:** Centralized computation of **Total Sales (₹3.02M+)**, **Average Order Value (~₹348)**, and processing of **8,680+ total orders**.
* **Temporal Trend Mapping:** Evaluation of order volumes distributed across Months/Quarters alongside cyclical weekly variations (**Daily Sales Trends**) to predict kitchen load requirements.
* **Geographic Revenue Distribution:** Identification of core revenue streams indicating **Mumbai (₹502K+)** and **Kolkata (₹487K+)** as leading delivery markets, backed by **Maharashtra** as the top-grossing state.
* **Dietary Segment Slicing:** A distinct breakdown revealing a massive consumer preference shift towards **Veg orders (₹2.87M)** over Non-veg alternatives within this dataset.

---

## 🗂️ Dataset Information & Data Dictionary

The project pipeline utilizes the raw transactional logs from `foodcourt_analysis.xlsx - swiggy.csv`:

| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| **ID** | Integer | Unique identifier code tracking each discrete order entry |
| **Area** | String | Local neighborhood or delivery sector zone |
| **City** | String | City tier classification where the restaurant operates |
| **State** | String | Geographical state locator (e.g., Maharashtra, Tamil Nadu, Karnataka) |
| **Restaurant** | String | Registered merchant name servicing the order |
| **Order Date** | Date | Calendar timeline indicator for transaction logging |
| **Price** | Integer | Total transaction monetary value (Order Cost) |
| **Avg ratings** | Float | Aggregated rating score given by historical customers (Scale: 1.0 - 5.0) |
| **Total ratings**| Integer | Volume weight of ratings left by consumers for that restaurant |
| **Dishes** | String | Tagged text string indicating menu items listed or bundled |
| **Food type** | String | Dietary classification tag (`Veg` or `Non-veg`) |
| **Address** | String | Granular destination street marker or landmark tags |
| **Delivery time**| Integer | Active logistical turnaround time metric captured in minutes |

### 📈 Workspace Architecture & Structure
* **Total Records Analyzed:** 8,680 individual rows.
* **Aggregations Built:** Customized data matrices segregating weekly patterns (`charts.csv`) and dedicated data blocks validating absolute baseline operational calculations (`kpi's.csv`).

---

## 🛠️ Tools & Technologies Used
* **Advanced Microsoft Excel / Sheets Data Engine:** Employed to isolate metrics, structural pivot lookups, and execute multi-dimensional cross-tabulations.
* **Analytical Modeling:** Segmented mapping techniques designed to parse nested food arrays into cleanly classified metric visualizations (`foodcourt_analysis.png`).

## 📂 Project Repository Structure
* `foodcourt_analysis.xlsx - swiggy.csv`: Cleaned transactional master logging.
* `foodcourt_analysis.xlsx - kpi's.csv`: Hardcoded calculations managing financial aggregations.
* `foodcourt_analysis.xlsx - charts.csv`: Time-series and categorical matrix feeds fueling the graphs.
* `foodcourt_analysis.png`: Complete snapshot showcasing the finalized reporting dashboard layout.
