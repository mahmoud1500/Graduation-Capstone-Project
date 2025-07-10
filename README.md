# 🚗 Car Rental Business Intelligence Dashboard – Capstone Project

## 🎓 Project Overview

This project was completed as part of my graduation capstone at Bellevue College's Business Intelligence program. The objective was to design and implement a robust data warehouse model and an interactive dashboard solution for a car rental business, enabling business stakeholders to make data-driven decisions and improve operational efficiency.

The project involved:
- Designing a star schema data warehouse
- Creating data visualizations to analyze fleet performance
- Building use case scenarios for multiple business personas
- Integrating a complete data flow from source to visualization

---

## 🧩 UML Diagram – Data Warehouse Schema

![UML Diagram](./OLAP%20UML%20Diagram.jpg)

This star schema includes:

- **FactPerformance**: Captures key performance metrics like revenue, ROI, utilization rate, average daily price, etc.
- **DimVehicle**: Vehicle attributes (Make, Model, Year, etc.)
- **DimDate**: Monthly and yearly date information
- **DimListing**: Customer interaction attributes like review and rating
- **DimLocation**: Geographic data (city and state)

This structure supports flexible and scalable analytics for reporting and decision-making.

---

## 📘 Use Case Diagram

![Use Case Diagram](./RCA%20Use%20Case%20Diagram.jpg)

### Actors and Use Cases:
- **Rental Company Executive**:
  - Analyzes rental trends, views city-level performance, and compares car segments
- **Rental Operator**:
  - Updates bookings and manages rental records and fleet
- **Data Engineer**:
  - Develops data warehouse, manages sources, and processes backend data
- **Data Visualization Developer**:
  - Designs and implements dashboards and visual filters

This diagram models real-world interactions with the system to ensure each stakeholder’s needs are addressed.

---

## 🔁 Sequence Diagram – Visualization Workflow

![Sequence Diagram](./Sequence%20Diagram%203%20last%20updated.png)

This diagram illustrates how data visualization developers interact with the data warehouse and dashboard components. It includes:
- Connection to data sources
- Processing and validation of rental data
- Feedback loops for improving visuals
- Scheduling data refresh
- UX feedback integration for layout adjustments

---

## 🌊 Data Flow Diagram

![Data Flow Diagram](./data%20flow%20diagram-%20last%20updated.png)

This diagram illustrates the end-to-end data flow for the car rental business intelligence solution, from data ingestion to final reporting. The process includes:
- **Data Scraping**: Raw listing data from the Turo Website.
- **Temporary Storage**: Raw data stored in an Excel Raw File.
- **Data Augmentation**: A Python script augments missing revenue data.
- **Data Cleaning and Normalization**: Car, location, and listing details are cleaned, formatted, and normalized.
- **Cleaned Data Storage**: Data is stored temporarily in an Excel Cleaned File.
- **Data Transfer**: SSIS is used to transfer cleaned data to the Azure Data Warehouse.
- **Data Analysis**: Queried data from the Data Warehouse is analyzed using Tableau.
- **Reporting**: Insights and charts are generated into reports for stakeholders (e.g., CEO).

---

## 🛠 Technologies Used

- **SQL Server / MySQL** – for data warehousing and querying
- **Tableau / Power BI** – for dashboard development
- **Excel** – for initial data modeling and validation
- **Draw.io** – for UML, sequence, and use case diagrams
- **Python (Optional)** – for preprocessing and ETL (if needed)
- **Azure Data Warehouse** - for scalable data storage
- **SSIS** - for data integration and transfer

---

## 📊 Key Features

- Multi-dimensional data warehouse using star schema
- Clean data model for vehicle rental metrics
- User-focused dashboard visualizations
- Support for trend analysis, ROI tracking, and fleet management
- Automated data flow from source to insights

---

## 🔗 Project Goal

To empower car rental businesses with the ability to:
- Monitor performance by location and vehicle segment
- Improve fleet utilization and ROI
- Make data-driven marketing and operational decisions

---

## 📁 Repository Structure

```bash
├── /diagrams/
│   ├── OLAP UML Diagram.jpg
│   ├── RCA Use Case Diagram.jpg
│   ├── Sequence Diagram 3 last updated.png
│   └── data flow diagram- last updated.png
├── /docs/
│   └── Capstone Report.pdf
├── README.md

