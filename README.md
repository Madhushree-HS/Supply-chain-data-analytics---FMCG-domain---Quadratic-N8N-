# 🧾Supply chain data analytics - FMCG domain - Quadratic | N8N |Supabase 

_A comprehensive analysis integrating sales transactions with supplier purchase data to optimize procurement, supplier relationships, and overall profitability._

---
## 📌 Table of Contents
- <a href="#overview">Overview</a>
- <a href="#problem-statement">Problem Statement</a>
- <a href="#dataset">Dataset</a>
- <a href="#tools--technologies">Tools & Technologies</a>
- <a href="#Method">Method</a>
- <a href="#key insights">Key-Insights</a>
- <a href="#System Architecture">System Architecture</a>
- <a href="#how-to-run-this-project">How to Run This Project</a>
- <a href="#final-recommendations">Final Recommendations</a>

---
<h2><a class="anchor" id="overview"></a>Overview</h2>
This project involved developing a comprehensive supply chain analytics system for AtliQ Mart, an FMCG manufacturer, using a modern no-code/low-code stack. The solution provided critical visibility into On-Time (OT), In-Full (IF), and On-Time In-Full (OTIF) delivery performance, enabling data-driven decisions that de-risked a major business expansion plan.

---
<h2><a class="anchor" id="problem-statement"></a>Problem-Statement</h2>

Mart was planning a significant business expansion but lacked a clear, data-driven understanding of its current delivery service levels to key customers. Without this insight, they risked expanding on a weak foundation, potentially leading to:
1.Severe financial penalties from large retailers for failing to meet strict OTIF targets
2.Loss of shelf space and damaged relationships with new and existing customers
3.Inefficient allocation of expansion capital due to unresolved underlying process issues

---
<h2><a class="anchor" id="dataset"></a>Dataset</h2>

**1. Order Data:** Order ID, Customer ID, Product ID, Order Date, Requested Quantity

**2. Delivery Data:** Delivery ID, Ship Date, Delivery Date, Delivered Quantity, Promised Delivery Date

**3. Customer Data:** Customer Name, Region, Customer Tier (Key vs. Standard)

**4. Product Data:** Product Name, Category

---

<h2><a class="anchor" id="tools--technologies"></a>Tools & Technologies</h2>

**Quadratic:** For spreadsheet-based data modeling, analysis, and KPI calculations

**N8N:** For workflow automation, data pipeline orchestration, and API integrations

**Supabase:** As the backend database for data storage, management, and real-time queries

**Excel:** For data visualization, reporting, and stakeholder presentations

---
<h2><a class="anchor" id="Method"></a>Method</h2>

**Data Pipeline Automation (N8N):**
      Set up automated workflows to collect and process data from various sources
      Configured data validation and transformation steps
      Automated data syncing between systems

**Data Storage & Management (Supabase):**
      Structured database schema for optimal query performance
      Implemented real-time data access and updates
      Set up secure API endpoints for data retrieval

**Data Analysis & KPI Calculation (Quadratic):**
      Built complex spreadsheet models with advanced formulas

**Calculated key metrics:**
      On-Time Delivery (OT)%: [On-Time Deliveries] / [Total Deliveries]
      In-Full Delivery (IF)%: [In-Full Deliveries] / [Total Deliveries]
      On-Time In-Full (OTIF)%: [On-Time & In-Full Deliveries] / [Total Deliveries]

**Reporting & Visualization (Excel):**
      Created dynamic dashboards with pivot tables and charts
      Built interactive reports with slicers and filters
      Developed automated reporting templates

---
<h2><a class="anchor" id="key-insights"></a>Key-insights</h2>

**Identification of Critical Weaknesses:** The analysis pinpointed 2-3 key customers where OTIF performance was critically low (<90%), which was previously masked by the overall company average

**Process Inefficiencies: **Revealed specific distribution centers and product categories contributing most to delays and shortages

**Quantified Risk: **Provided a clear benchmark showing that expanding with the current service levels would result in an estimated loss of 20% of the expansion investment due to penalties and lost sales

---
<h2><a class="anchor" id="System Architecture"></a>System Architecture</h2>

**Data Ingestion Layer:** N8N workflows for automated data collection

**Data Storage Layer:** Supabase database with optimized schema

**Filters & Interactivity:** Customer, Region, Time Period selectors

**Performance Metrics:** OT%, IF%, OTIF% tracking

**Trend Analysis:** Historical performance charts

---
<h2><a class="anchor" id="how-to-run-this-project"></a>How to Run This Project</h2>

**Prerequisites:**
      Quadratic account and workspace
      N8N instance (cloud or self-hosted)
      Supabase project setup
      Excel with data connections configured

**Data Setup:**
      Configure N8N workflows to connect to your data sources
      Set up Supabase tables with the required schema
      Establish data connections between all components

**System Initialization:**
      Run N8N workflows to populate Supabase with initial data
      Connect Quadratic to Supabase via API
      Refresh Excel data connections to pull analyzed data

**Ongoing Operation:**
      N8N automates daily data syncs
      Quadratic processes and analyzes updated data
      Excel dashboards refresh automatically for daily reporting

---
<h2><a class="anchor" id="final-recommendations"></a>Final Recommendations</h2>

**Immediate Customer Engagement:** Proactively meet with identified key customers with low OTIF% to address specific issues and rebuild trust before expansion

**Process Optimization:** Focus improvement efforts on specific distribution centers and product lines causing the most significant delays

**System Scaling:** Leverage the current tech stack to build additional monitoring capabilities as the business grows

**Postpone Scaling Until Stable:** Delay the expansion launch until OTIF% for key accounts is consistently above 98%, thereby protecting the planned investment and ensuring successful scale-up


---



