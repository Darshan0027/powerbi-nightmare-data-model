# Power BI Data Modeling – Nightmare Data Model

## 📌 Project Overview

An end-to-end Power BI data modeling project focused on transforming 23 messy source tables into a clean, scalable, and optimized analytical data model.

The project implements a multi-fact star schema architecture to handle complex business processes including sales, inventory, campaigns, order processing, and promotions, creating a structured Power BI semantic model suitable for comprehensive business reporting.

## 🎯 Project Objectives

- Explore and understand 23 complex, unstructured source tables
- Separate transactional events into distinct fact tables and descriptive attributes into dimensions
- Design a clean, high-performance star schema data model
- Establish correct table relationships, cardinalities, and filter directions
- Build a centralized Date dimension and reusable supporting dimensions
- Create calculated measures using DAX
- Validate relationships and build a business-ready Power BI semantic model

## 🏗️ Data Modeling Approach

The original dataset consisted of 23 unstructured source tables. Through data cleansing and transformation, these tables were re-architected into a robust multi-fact star schema framework.

### Dimension Tables

- **`dim_customer`** — Customer master details and attributes
- **`dim_product`** — Product catalog details, categories, and branding
- **`dim_date`** — Centralized calendar table for time intelligence
- **`dim_geo`** — Geographic location attributes such as City and Region
- **`dim_campaign`** — Marketing campaign metadata
- **`dim_order_flags`** — Standardized lookup for order statuses, channels, and priorities
- **Security & Standalone Tables** — Supporting security mappings and calculated metrics

### Fact Tables

- **`fact_sales`** — Core transactional sales data including orders, quantities, and pricing
- **`fact_inventory`** — Stock levels and product inventory metrics
- **`fact_order_process`** — Order lifecycle tracking including fulfillment, delivery, and payment timelines
- **`fact_campaign_spent`** — Marketing performance tracking including clicks, impressions, and spend
- **`fact_promotion_coverage`** — Mapping between active campaigns and promoted products
- **`fact_sale_target`** — Revenue and sales targets

## 🔄 Before vs After Modeling

### Before Modeling

The original setup consisted of 23 source tables with complex relationships and dependencies.

![Before Modeling](Before_modeling.png)

### After Modeling

The final model was reorganized into a structured multi-fact star schema with clear relationships between fact and dimension tables.

![After Modeling](After_modeling.png)

## ⭐ Star Schema & Architecture

The final model utilizes a **multi-fact star schema** design pattern:

- **Fact Tables** capture quantifiable transactional business events such as sales, inventory, order processing, and campaign spending at their appropriate grains.
- **Dimension Tables** such as Customer, Product, Geography, Date, and Campaign provide descriptive attributes for filtering and analyzing the fact data.
- Common dimensions are shared across multiple fact tables where appropriate.
- Relationships are structured using appropriate cardinality and filter directions to support predictable filter propagation and analytical reporting.

## 🧠 Key Concepts Implemented

- Multi-Fact Star Schema Architecture
- Dimensional Modeling
- Fact vs. Dimension Separation
- Primary & Foreign Key Management
- Table Relationships & Cardinality
- One-to-Many Relationships
- Filter Direction
- Time Intelligence & Date Dimension
- DAX Measures
- Calculated Columns
- Power Query Data Transformation
- Power BI Semantic Model Design
- Data Validation

## 🛠️ Tools & Technologies

- **Power BI Desktop**
- **Power Query** — Data Transformation & ETL
- **DAX** — Data Analysis Expressions
- **Dimensional Data Modeling**

## 📚 Key Learning Outcomes

- Transforming messy enterprise-style schemas into clean, report-ready analytical models
- Handling multiple fact tables sharing common dimensions
- Understanding and defining the correct grain of fact tables
- Preventing incorrect aggregation and data duplication
- Designing relationship paths for predictable filter propagation
- Applying star-schema principles in Power BI
- Building a structured semantic model for business reporting

## 📂 Project Files

- [Before Modeling Image](Before_modeling.png)
- [After Modeling Image](After_modeling.png)
- [Power BI Project File](Data%20Modeling%20Project.pbix)

## 🔗 Reference

This project was completed as a practical learning exercise based on the **Power BI Data Modeling / Nightmare Data Model** project by Data with Baraa.
