# ✈️ Aviation Data Career Guide
## 40 Airline Analysis Projects — Ranked by Role, Difficulty & Portfolio Value

> **For:** Job seekers targeting aviation industry data roles  
> **Skills assumed:** SQL (intermediate) · Python (intermediate) · Willingness to learn  
> **Source projects:** *How to Analyze an Airline Company* — Umbrex / Will Bachman (2024)

---

## 📋 Table of Contents

- [How to Use This Guide](#how-to-use-this-guide)
- [Role Definitions and Skill Expectations](#role-definitions-and-skill-expectations)
- [Difficulty Legend](#difficulty-legend)
- [🔵 Data Analyst — Project Rankings](#-data-analyst--project-rankings)
  - [Easy Projects (Start Here)](#-easy-projects-start-here)
  - [Medium Projects (Build Momentum)](#-medium-projects-build-momentum)
  - [Hard Projects (Stretch Goals)](#-hard-projects-stretch-goals)
  - [⭐ Top 5 Portfolio Projects for Data Analysts](#-top-5-portfolio-projects-for-data-analysts)
- [🟠 Data Engineer — Project Rankings](#-data-engineer--project-rankings)
  - [Easy Projects (Start Here)](#-easy-projects-start-here-1)
  - [Medium Projects (Build Momentum)](#-medium-projects-build-momentum-1)
  - [Hard Projects (Stretch Goals)](#-hard-projects-stretch-goals-1)
  - [⭐ Top 5 Portfolio Projects for Data Engineers](#-top-5-portfolio-projects-for-data-engineers)
- [🟢 Data Scientist — Project Rankings](#-data-scientist--project-rankings)
  - [Easy Projects (Start Here)](#-easy-projects-start-here-2)
  - [Medium Projects (Build Momentum)](#-medium-projects-build-momentum-2)
  - [Hard Projects (Stretch Goals)](#-hard-projects-stretch-goals-2)
  - [⭐ Top 5 Portfolio Projects for Data Scientists](#-top-5-portfolio-projects-for-data-scientists)
- [Master Comparison Table — All 40 Projects](#master-comparison-table--all-40-projects)
- [Public Datasets to Build Your Portfolio](#public-datasets-to-build-your-portfolio)
- [Suggested Learning Path by Role](#suggested-learning-path-by-role)
- [Interview Talking Points by Project](#interview-talking-points-by-project)

---

## How to Use This Guide

Each of the 40 airline analysis projects from the source document has been evaluated across three dimensions **for each role**:

| Dimension | What it means |
|---|---|
| **Ease** | How achievable is this with SQL + Python at your current level? |
| **Portfolio Value** | How impressive is a completed version of this to an aviation hiring manager? |
| **Career Signal** | What does this project prove about you as a candidate? |

Work through **Easy projects first** to build domain knowledge and get comfortable with airline-specific metrics (RPK, ASK, load factor, yield). Then tackle **Medium projects** for portfolio pieces. Use **Hard projects** as aspirational goals once you land a junior role.

The `⭐ Portfolio Projects` sections are the ones you should actually build and publish on GitHub before applying.

---

## Role Definitions and Skill Expectations

### 🔵 Data Analyst
> Turns raw data into dashboards, reports, and business insights for operations and strategy teams.

**Day-to-day tools:** SQL, Python (pandas, matplotlib, seaborn), Excel, Tableau or Power BI  
**Core deliverables:** KPI dashboards, ad hoc reports, trend analysis, revenue/cost summaries  
**Aviation-specific focus:** Load factors, on-time performance, route profitability, ancillary revenue  

---

### 🟠 Data Engineer
> Builds and maintains the data infrastructure that powers every other data role.

**Day-to-day tools:** Python (PySpark, Airflow, SQLAlchemy), SQL, cloud platforms (AWS/GCP/Azure), dbt, Kafka  
**Core deliverables:** ETL pipelines, data warehouse schemas, real-time data feeds, data quality checks  
**Aviation-specific focus:** Integrating flight ops systems, revenue management systems, MRO systems into a unified warehouse  

---

### 🟢 Data Scientist
> Builds predictive models, optimizes decisions, and extracts forward-looking insights from data.

**Day-to-day tools:** Python (scikit-learn, XGBoost, statsmodels, TensorFlow), SQL, Jupyter, MLflow  
**Core deliverables:** Forecasting models, classification models, optimization algorithms, A/B test analysis  
**Aviation-specific focus:** Demand forecasting, dynamic pricing, predictive maintenance, fraud detection  

---

## Difficulty Legend

| Symbol | Level | Meaning for SQL + Python job seekers |
|---|---|---|
| 🟢 | **Easy** | Achievable now — uses pandas, basic SQL, matplotlib. Can be completed in a weekend. |
| 🟡 | **Medium** | Achievable in 1–2 weeks — requires multi-table SQL, intermediate Python, some domain research. |
| 🔴 | **Hard** | Requires significant upskilling — involves optimization, ML modeling, real-time systems, or advanced statistics. |

---

## 🔵 Data Analyst — Project Rankings

> **Your goal as a DA:** Build dashboards and reports that measure airline performance KPIs. Your SQL and Python are your primary tools. Focus on projects with clear metrics, structured outputs, and business storytelling.

---

### 🟢 Easy Projects (Start Here)

These projects are achievable with SQL aggregations, pandas DataFrames, and matplotlib/seaborn charts. They produce clear, visual outputs that work well in a portfolio.

---

#### 🟢 #10 · Fuel Efficiency per Aircraft Type Analysis
**Why it's easy:** You're comparing a single metric (fuel consumed per RPK/ASK) across aircraft types. Simple GROUP BY SQL queries + bar/scatter charts.  
**What you build:** A comparison table and chart ranking aircraft by fuel efficiency  
**SQL skills used:** `GROUP BY`, `AVG()`, `SUM()`, window functions  
**Python skills used:** pandas, seaborn bar plot, matplotlib annotations  
**Domain value:** Demonstrates you understand one of the airline industry's #1 cost drivers  

---

#### 🟢 #12 · Pilot Training and Simulator Utilization Analysis
**Why it's easy:** Straightforward utilization rate calculation. Clean scheduling data, simple ratios.  
**What you build:** A utilization heatmap by day/hour + a training cost breakdown table  
**SQL skills used:** `DATE_PART`, `GROUP BY`, `CASE WHEN` for peak/off-peak labeling  
**Python skills used:** pandas pivot tables, seaborn heatmap  
**Domain value:** Shows you understand operational workforce planning  

---

#### 🟢 #15 · On-Time Performance and Operational Reliability Analysis
**Why it's easy:** The primary metric (% of flights on time) is a simple count/total ratio. Delay causes are a categorical breakdown.  
**What you build:** An OTP dashboard with delay cause breakdown, route-level performance, and time-of-day analysis  
**SQL skills used:** `COUNT`, `CASE WHEN`, `GROUP BY` route/carrier/time  
**Python skills used:** pandas, seaborn bar chart, pie chart for delay causes  
**Domain value:** Airlines are obsessed with OTP. This shows immediate industry fluency.  
**Public data tip:** U.S. Bureau of Transportation Statistics publishes free monthly OTP data  

---

#### 🟢 #13 · Load Factor and Capacity Management Analysis
**Why it's easy:** Load factor = RPK / ASK × 100. This is THE core aviation metric and most public datasets include it directly.  
**What you build:** Route-level load factor trends by season, comparison to break-even load factor  
**SQL skills used:** `SUM`, `GROUP BY`, `HAVING`, CTEs for seasonal aggregation  
**Python skills used:** pandas, line charts for trends, heatmap for route × season matrix  
**Domain value:** This is the single most important operational metric for airline analysts. Knowing it deeply signals industry readiness.  
**Public data tip:** U.S. DOT T-100 database has ASM and RPM data by carrier, route, and month  

---

#### 🟢 #3 · Route Profitability and Market Share Analysis
**Why it's easy:** The formulas are straightforward. The data requirements (revenue, cost, load factor per route) are all computable from public DOT databases.  
**What you build:** A ranked route profitability table, market share bar chart vs. competitors, seasonal demand overlay  
**SQL skills used:** `JOIN` across route, revenue, and cost tables; CTEs; window functions (`RANK()`)  
**Python skills used:** pandas, matplotlib stacked bar chart, scatter plot (load factor vs. yield)  
**Domain value:** Route profitability is the most fundamental financial question an airline asks about its network.  

---

#### 🟢 #4 · Seasonal Demand and Network Flexibility Analysis
**Why it's easy:** Time series aggregation by month/quarter. Seasonal patterns are visible with simple line charts.  
**What you build:** Monthly/quarterly load factor trends by route, seasonal demand index, capacity vs. demand gap chart  
**SQL skills used:** `DATE_TRUNC`, `GROUP BY month`, `LAG()` for year-over-year comparison  
**Python skills used:** pandas, matplotlib line charts, seaborn seasonal decomposition  
**Domain value:** Shows you understand cyclical demand patterns — relevant for scheduling, pricing, and capacity teams  

---

#### 🟢 #25 · Passenger Yield and Demographic Analysis
**Why it's easy:** Yield = Revenue / RPK. Demographic segmentation uses simple GROUP BY queries on customer attributes.  
**What you build:** Yield comparison by route and cabin class, demographic breakdown chart, seasonal yield trends  
**SQL skills used:** `GROUP BY`, `AVG`, `PERCENTILE_CONT`, `CASE WHEN` for segment labeling  
**Python skills used:** pandas, box plots for yield distribution, bar charts by demographic  
**Domain value:** Revenue management teams care deeply about yield optimization. This signals commercial awareness.  

---

#### 🟢 #8 · Fleet Utilization and Efficiency Analysis
**Why it's easy:** Utilization rate = flight hours / available days. Straightforward aggregation by aircraft type.  
**What you build:** Aircraft utilization rate table, CASK comparison by aircraft, fuel burn vs. utilization scatter plot  
**SQL skills used:** `GROUP BY aircraft_type`, `SUM flight_hours`, `AVG CASK`  
**Python skills used:** pandas, seaborn scatter plots, bar charts  
**Domain value:** Fleet efficiency is a core operations analytics responsibility  

---

#### 🟢 #27 · Loyalty Program Redemption Cost and Breakage Rate Analysis
**Why it's easy:** Two formulas (redemption cost per point, breakage rate). Clear inputs, clean business interpretation.  
**What you build:** Breakage rate by tier, redemption cost by reward type, trend line over time  
**SQL skills used:** `SUM`, `GROUP BY tier`, `LAG()` for breakage trend  
**Python skills used:** pandas, stacked bar chart by tier, line chart for breakage rate over time  
**Domain value:** Loyalty programs are a multi-billion dollar revenue line for airlines. Shows commercial analytics depth.  

---

#### 🟢 #30 · Environmental Compliance and Sustainability Strategy
**Why it's easy:** Emissions calculations use simple multiplication formulas. Data sources are often publicly available (ICAO, EPA).  
**What you build:** Emissions by route and aircraft table, fuel efficiency vs. emissions scatter, sustainability benchmarking chart  
**SQL skills used:** `GROUP BY`, `SUM(fuel * emission_factor)`, `JOIN` to benchmarks  
**Python skills used:** pandas, scatter plots, bar comparison vs. industry benchmark  
**Domain value:** ESG and sustainability are top priorities for airline leadership. Differentiates you from candidates who only know financial metrics.  

---

#### 🟢 #26 · In-Flight Service and Product Differentiation Analysis
**Why it's easy:** Mostly descriptive analysis of satisfaction scores and revenue per service. No complex modeling.  
**What you build:** NPS/satisfaction comparison by cabin class, revenue vs. cost per service chart, competitive benchmarking table  
**SQL skills used:** `AVG`, `GROUP BY cabin_class`, `JOIN` satisfaction to revenue data  
**Python skills used:** pandas, seaborn bar charts, bubble charts (revenue vs. satisfaction vs. cost)  
**Domain value:** Customer experience analytics is increasingly important for premium airline products  

---

#### 🟢 #32 · Safety and Incident Reporting Compliance Analysis
**Why it's easy:** Incident trend analysis is categorical and time-based aggregation. Clear regulatory benchmarks to compare against.  
**What you build:** Incident frequency trend line, cause breakdown chart, compliance audit scorecard  
**SQL skills used:** `COUNT`, `GROUP BY incident_type, severity`, `DATE_TRUNC`  
**Python skills used:** pandas, seaborn, heatmap (incident type × severity matrix)  
**Domain value:** Safety analytics is a regulated, mandatory function at every airline — shows professionalism  

---

### 🟡 Medium Projects (Build Momentum)

These require multi-source data, more complex SQL (window functions, CTEs, multiple JOINs), and Python analysis that goes beyond basic charts.

---

#### 🟡 #6 · Competitor Route Overlap and Market Penetration Analysis
**Why it's medium:** Requires combining your airline's data with competitor data from public sources (BTS, OAG). Market share calculation needs careful data modeling.  
**What you build:** Market share comparison dashboard, competitor pricing heatmap, route overlap map  
**SQL skills needed:** `FULL OUTER JOIN`, `CASE WHEN`, window functions `RANK()`, `LAG()`  
**Python skills needed:** pandas, competitive positioning scatter plot, optionally: folium for map  

---

#### 🟡 #23 · Ancillary Revenue and Additional Services Yield Management
**Why it's medium:** Requires segmenting revenue by service type AND passenger type AND route — a multi-dimensional analysis requiring careful data modeling.  
**What you build:** Ancillary revenue breakdown by service, passenger segment purchase behavior analysis, seasonal demand chart  
**SQL skills needed:** Multi-table joins, `PIVOT`, `GROUP BY ROLLUP`  
**Python skills needed:** pandas pivot tables, grouped bar charts, seaborn heatmap  

---

#### 🟡 #14 · MRO Cost Analysis
**Why it's medium:** Requires connecting maintenance schedule data to cost data to downtime data across multiple systems.  
**What you build:** MRO cost breakdown table, in-house vs. outsourced comparison, downtime revenue impact calculator  
**SQL skills needed:** CTEs, multi-table joins, `CASE WHEN` for cost categorization  
**Python skills needed:** pandas, waterfall chart for cost breakdown, matplotlib  

---

#### 🟡 #21 · Passenger Flow and Boarding Process Efficiency Analysis
**Why it's medium:** Requires timestamp-level data and derived time calculations. Bottleneck detection needs more careful logic.  
**What you build:** Boarding time comparison by method, passenger flow funnel chart, load vs. boarding time correlation  
**SQL skills needed:** `DATEDIFF`, `LAG`, timestamp arithmetic, `GROUP BY boarding_zone`  
**Python skills needed:** pandas, funnel chart, scatter plot with regression line  

---

#### 🟡 #35 · Airport and Route-Level Cost Structure Analysis
**Why it's medium:** CASM calculation requires joining operational schedule data with detailed cost breakdowns.  
**What you build:** CASM comparison by route, airport cost breakdown table, high-cost route ranking  
**SQL skills needed:** Multi-table joins, window functions `NTILE()` for cost quartiles, CTEs  
**Python skills needed:** pandas, horizontal bar chart, scatter (CASM vs. profitability)  

---

#### 🟡 #18 · Cabin Configuration and Seat Density Optimization
**Why it's medium:** Requires revenue per seat calculation across cabin classes combined with satisfaction survey data — two different source systems.  
**What you build:** Revenue per seat by cabin class chart, seat density vs. satisfaction scatter, reconfiguration ROI estimate  
**SQL skills needed:** `JOIN` seat config to revenue to satisfaction data, `CASE WHEN` for class segmentation  
**Python skills needed:** pandas, dual-axis chart (revenue + satisfaction), break-even calculation  

---

#### 🟡 #24 · Cargo Revenue and Capacity Utilization Analysis
**Why it's medium:** Cargo-specific metrics (RTK, ACTK) are less familiar. Requires understanding cargo data schema on top of passenger data.  
**What you build:** Cargo load factor by route, revenue per RTK trend, seasonal capacity vs. demand chart  
**SQL skills needed:** `GROUP BY`, `SUM`, `RATIO_TO_REPORT`, CTEs  
**Python skills needed:** pandas, dual-axis seasonal chart, route ranking by profitability  

---

#### 🟡 #31 · De-icing and Weather Contingency Cost Analysis
**Why it's medium:** Requires joining weather event data with operational and cost data — a real-world data integration challenge.  
**What you build:** De-icing cost by airport and season, weather delay correlation chart, passenger compensation cost analysis  
**SQL skills needed:** `JOIN` weather events to flight operations, date-range matching  
**Python skills needed:** pandas, seaborn correlation heatmap, matplotlib seasonal bar chart  

---

#### 🟡 #38 · Alliance and Codeshare Partnership Evaluation
**Why it's medium:** Requires attributing revenue splits across partners and segmenting by alliance vs. non-alliance flights.  
**What you build:** Revenue contribution table by partner, load factor comparison for alliance vs. non-alliance routes  
**SQL skills needed:** `JOIN` across multiple partner datasets, `CASE WHEN` for alliance labeling  
**Python skills needed:** pandas, grouped comparison charts  

---

#### 🟡 #5 · Market Entry and Route Launch Feasibility Analysis
**Why it's medium:** Requires building a demand forecast (even a simple regression or trend extrapolation) and a projected P&L table.  
**What you build:** Demand forecast chart, projected route profitability model, risk matrix table  
**SQL skills needed:** Aggregation of comparable routes, `PERCENTILE_CONT` for benchmarking  
**Python skills needed:** pandas, simple linear regression (scikit-learn), matplotlib  

---

#### 🟡 #29 · Customer Satisfaction Analysis of Airline Loyalty Programs
**Why it's medium:** Requires NPS calculation, churn rate analysis, and cross-referencing satisfaction data with behavioral data.  
**What you build:** NPS by tier, churn rate trend, satisfaction driver waterfall chart  
**SQL skills needed:** Cohort retention query, `DATE_TRUNC` for monthly churn, `AVG(NPS)`  
**Python skills needed:** pandas, cohort retention heatmap, waterfall chart  

---

### 🔴 Hard Projects (Stretch Goals)

These are aspirational for a junior/entry-level analyst. Tackle these after landing your first aviation data role.

---

#### 🔴 #1 · Route Network and Hub Optimization Analysis
**Why it's hard:** Requires graph analysis of the full network. True hub optimization involves operations research, not just SQL aggregation.  
**Skills gap:** NetworkX graph analysis, routing algorithms  

---

#### 🔴 #22 · Core Services Revenue and Dynamic Pricing Analysis
**Why it's hard:** Building a working dynamic pricing model requires understanding revenue management systems, price elasticity modeling, and real-time data feeds.  
**Skills gap:** Price elasticity estimation, revenue management theory, real-time data architecture  

---

#### 🔴 #34 · Debt Structure and Lease Obligations Review
**Why it's hard:** This is corporate finance territory requiring advanced financial modeling (DCF, sensitivity tables) and knowledge of accounting standards for leases.  
**Skills gap:** Financial modeling, IFRS 16/ASC 842 lease accounting  

---

#### 🔴 #40 · IT and Digital Transformation Capability Assessment
**Why it's hard:** This is more a consulting/strategy deliverable than a data analysis. Requires deep systems knowledge and stakeholder interviews.  
**Skills gap:** Enterprise IT architecture, technology maturity frameworks  

---

### ⭐ Top 5 Portfolio Projects for Data Analysts

> Build these, publish them on GitHub with clean README files, and reference them in every airline job application.

---

#### ⭐ Portfolio Project 1: Airline On-Time Performance Dashboard
**Based on Analysis #15**

**What to build:** An end-to-end analysis using the U.S. Bureau of Transportation Statistics (BTS) On-Time Performance dataset. Clean the data with Python, store it in a local SQLite or PostgreSQL database, query it with SQL, and visualize it with matplotlib/seaborn or a Tableau Public dashboard.

**Deliverables:**
- Jupyter Notebook with full SQL + Python analysis
- Interactive Tableau/Power BI dashboard (publish to Tableau Public)
- GitHub README explaining methodology and findings

**Skills demonstrated:** SQL querying, data cleaning, KPI measurement, data visualization, storytelling  
**Why it impresses:** BTS data is what real airline analysts use. Using it shows you already know the industry's data sources.  
**Dataset:** [BTS On-Time Performance](https://www.transtats.bts.gov/OT_Delay/OT_DelayCause1.asp)  

---

#### ⭐ Portfolio Project 2: U.S. Route Profitability & Market Share Explorer
**Based on Analysis #3**

**What to build:** Using BTS T-100 and DB1B fare data, build a route-level profitability and market share analysis for 2–3 major U.S. carriers.

**Deliverables:**
- SQL scripts to build a clean route-level fact table
- Python analysis of yield, load factor, and market share
- Visual comparison of 2–3 airlines on overlapping routes

**Skills demonstrated:** Multi-source data joining, aviation KPI fluency (RPK, ASK, yield, load factor), competitive analysis  
**Why it impresses:** Shows you can answer the #1 question every airline commercial team has: "Are we making money on this route?"  
**Datasets:** [BTS T-100 Segment Data](https://www.transtats.bts.gov/) + [DB1B Fare Database](https://www.transtats.bts.gov/DatabaseInfo.asp?QO_VQ=EFD)  

---

#### ⭐ Portfolio Project 3: Airline Sustainability & Emissions Report
**Based on Analysis #30**

**What to build:** Calculate and visualize CO₂ emissions per available seat kilometer (ASK) for major U.S. carriers, using fuel consumption reports and ICAO emission factors. Benchmark against industry targets.

**Deliverables:**
- Python analysis of emissions intensity by carrier and fleet type
- Trend analysis showing emissions improvement (or regression) over 5 years
- A clean HTML or Markdown report with charts embedded

**Skills demonstrated:** Environmental data analysis, Python scripting, business report writing  
**Why it impresses:** ESG analytics is a rapidly growing function at airlines. This differentiates you from candidates who only know financial KPIs. It also shows initiative — most junior candidates don't think about this.  

---

#### ⭐ Portfolio Project 4: Seasonal Load Factor & Capacity Planning Model
**Based on Analysis #4 + #13**

**What to build:** A combined seasonal demand and capacity analysis. Use 3–5 years of monthly BTS data to show how load factors shift by season, identify over/under-capacity routes, and calculate the revenue opportunity of better capacity alignment.

**Deliverables:**
- SQL pipeline pulling monthly load factor data into a structured table
- Python seasonal decomposition (STL or rolling averages)
- Revenue opportunity calculation: "If route X matched competitor's load factor, additional revenue = $Y"

**Skills demonstrated:** Time series thinking, SQL pipeline, business quantification, aviation KPI depth  
**Why it impresses:** Combines two of the most-asked questions in airline analytics into one cohesive story. The "revenue opportunity" calculation shows business impact thinking.  

---

#### ⭐ Portfolio Project 5: Airline Loyalty Program Breakage & Retention Analysis
**Based on Analysis #27 + #29**

**What to build:** Simulate a loyalty program dataset (or use publicly available airline loyalty disclosures) to analyze breakage rates, redemption patterns by tier, and cohort retention.

**Deliverables:**
- Python synthetic data generation script (or data from airline annual reports)
- SQL cohort retention analysis
- Breakage rate calculation and business impact quantification

**Skills demonstrated:** SQL cohort analysis, loyalty program KPIs, financial impact quantification  
**Why it impresses:** Loyalty programs generate 10–30% of airline revenue through partnerships. Showing you understand this signals commercial maturity.  

---

## 🟠 Data Engineer — Project Rankings

> **Your goal as a DE:** Build pipelines, schemas, and infrastructure that power all data work. Think about data flow, reliability, scalability, and integration. Your SQL is for schema design and transformation logic; Python is for orchestration, pipeline code, and data quality.

---

### 🟢 Easy Projects (Start Here)

---

#### 🟢 #10 · Fuel Efficiency per Aircraft Type — Data Pipeline
**Why it's easy for DE:** Clean source structure. Simple pipeline: ingest aircraft fuel logs → transform to efficiency metrics → load to warehouse table.  
**What you build:** An Airflow DAG (or simple Python script) that reads raw fuel consumption CSVs, calculates efficiency metrics, and writes to a structured PostgreSQL table  
**Pipeline skills used:** Python ETL script, pandas transforms, SQLAlchemy for DB writes  
**Schema design:** `fact_fuel_efficiency (aircraft_type, route_id, date, fuel_per_rpk, fuel_per_ask)`  

---

#### 🟢 #12 · Pilot Training Utilization — Scheduling Data Pipeline
**Why it's easy for DE:** Scheduling data has a clean structure (start time, end time, simulator ID, pilot ID). A straightforward ETL with datetime processing.  
**What you build:** A pipeline that ingests training schedule records and computes daily utilization rates, written to a reporting table  
**Pipeline skills used:** Python datetime parsing, pandas, SQLAlchemy  
**Schema design:** `fact_simulator_utilization (simulator_id, date, hours_used, hours_available, utilization_rate)`  

---

#### 🟢 #32 · Safety and Incident Reporting — Compliance Data Pipeline
**Why it's easy for DE:** Incident reports are usually structured or semi-structured (JSON/CSV). Good exercise in data validation and quality checks.  
**What you build:** A pipeline that ingests incident reports, validates required fields, standardizes severity categories, and loads to a compliance schema  
**Pipeline skills used:** Python, data validation (Great Expectations or custom checks), pandas  
**Schema design:** `fact_safety_incidents (incident_id, date, aircraft_type, route_id, severity, cause_category, status)`  

---

#### 🟢 #26 · In-Flight Service Revenue — Simple Aggregation Pipeline
**Why it's easy for DE:** Ancillary revenue data from in-flight sales is transactional. Clean, well-structured records. Great pipeline fundamentals exercise.  
**What you build:** A pipeline ingesting in-flight purchase transactions, aggregating to route/flight/service level, loading to a reporting table  
**Pipeline skills used:** Python, pandas, SQL aggregations, basic schema design  

---

### 🟡 Medium Projects (Build Momentum)

---

#### 🟡 #15 · On-Time Performance — Multi-Source Integration Pipeline
**Why it's medium:** OTP data comes from multiple systems: flight operations (actual times), scheduling systems (planned times), ATC delay reasons, and weather feeds. Joining them correctly is the challenge.  
**What you build:** A pipeline that ingests flight schedule data, actual departure/arrival timestamps, and delay cause codes — joins them, calculates OTP metrics, and writes to a warehouse  
**Pipeline skills used:** Python, multi-source joins, data reconciliation logic, schema design  
**Schema design:** `fact_flight_performance (flight_id, date, route_id, scheduled_dep, actual_dep, delay_minutes, delay_cause_code, is_on_time)`  
**Why it matters:** Demonstrates multi-system data integration — the core competency of airline data engineering  

---

#### 🟡 #13 · Load Factor — Real-Time Capacity Tracking Pipeline
**Why it's medium:** Load factor ideally updates in near-real-time as bookings come in. Requires connecting a bookings stream to capacity data.  
**What you build:** A pipeline reading booking records incrementally, joining to flight capacity, computing current load factor per flight, and updating a monitoring table  
**Pipeline skills used:** Python, incremental loading pattern, upsert logic in SQL, optional: Kafka for streaming  
**Schema design:** `fact_flight_capacity (flight_id, date, route_id, seats_available, seats_booked, load_factor, last_updated)`  

---

#### 🟡 #14 · MRO Cost Data Warehouse
**Why it's medium:** MRO data comes from multiple specialized systems (maintenance management software, parts inventory, labor tracking). Designing the schema to unify these is the challenge.  
**What you build:** A dimensional model for MRO data — fact table for maintenance events, dimensions for aircraft, maintenance type, parts, labor  
**Pipeline skills used:** dbt for transformations, dimensional modeling, SQL, Python ingestion scripts  
**Schema design:** Star schema — `fact_maintenance_event` + `dim_aircraft`, `dim_maintenance_type`, `dim_airport`, `dim_date`  
**Why it matters:** Dimensional modeling for operational data is a classic data engineering interview topic  

---

#### 🟡 #3 · Route Profitability — Financial Data Warehouse Schema
**Why it's medium:** Revenue and cost data often live in separate systems (revenue management vs. finance/ERP). Building a reliable route-level P&L requires careful reconciliation logic.  
**What you build:** A schema and dbt project that joins revenue (from booking system), variable costs (from ops system), and fixed cost allocations (from finance ERP) into a route-level profitability fact table  
**Pipeline skills used:** dbt models, SQL CTEs, data reconciliation tests, schema documentation  
**dbt model structure:** `stg_bookings` → `stg_costs` → `int_route_revenue` → `int_route_costs` → `fct_route_profitability`  

---

#### 🟡 #25 · Passenger Yield & Demographic — CRM Data Integration
**Why it's medium:** Requires integrating booking system data (transactional) with CRM/loyalty data (customer attributes). Privacy/PII handling is an important consideration.  
**What you build:** A pipeline that safely joins anonymized booking records to loyalty profile attributes, building a customer-level yield fact table  
**Pipeline skills used:** Python, PII masking/hashing, schema design, SQL joins  
**Schema design:** `fact_passenger_yield (hashed_customer_id, flight_id, cabin_class, ticket_revenue, rpk, yield, demographic_segment)`  

---

#### 🟡 #4 · Seasonal Demand — Automated Reporting Pipeline
**Why it's medium:** Requires scheduling automated monthly refreshes, handling late-arriving data (flights that get updated after the fact), and ensuring data backfill works correctly.  
**What you build:** An Airflow DAG that runs monthly to refresh seasonal load factor and demand metrics, with data quality checks and email alerts for anomalies  
**Pipeline skills used:** Apache Airflow, Python operators, SQL transforms, data quality checks, alerting  
**Why it matters:** Orchestration with Airflow is one of the most requested DE skills in job descriptions  

---

#### 🟡 #29 · Loyalty Program — Cohort Retention Data Model
**Why it's medium:** Cohort analysis requires point-in-time snapshots of member status. Slowly Changing Dimensions (SCD Type 2) are needed to track tier changes over time.  
**What you build:** A loyalty program data model with SCD Type 2 for member tier history, and SQL logic to compute monthly cohort retention  
**Pipeline skills used:** SCD Type 2 implementation, Python upsert logic, dbt snapshots  
**Schema design:** `dim_member_scd (member_id, tier, valid_from, valid_to, is_current)` + `fact_member_activity`  
**Why it matters:** SCD Type 2 is a classic data engineering interview question  

---

#### 🟡 #36 · Fuel Tankering — Cost Optimization Data Feed
**Why it's medium:** Requires ingesting real-time (or near-real-time) fuel price data from external sources and joining to flight schedule data to compute tankering opportunities.  
**What you build:** A pipeline that pulls fuel price data from an API or daily feed, joins to the flight schedule, computes net tankering savings per flight, and writes to a decision-support table  
**Pipeline skills used:** API data ingestion, Python requests, joins to internal data, scheduled refreshes  

---

#### 🟡 #38 · Alliance Codeshare — Multi-Partner Data Integration
**Why it's medium:** Alliance data comes from partner airlines in different formats. Standardizing schemas across partners and reconciling revenue splits is the core engineering challenge.  
**What you build:** A pipeline that ingests codeshare booking data from 2–3 partners in different formats (CSV, JSON, XML), normalizes to a common schema, and loads to an alliance revenue fact table  
**Pipeline skills used:** Multi-format ingestion, schema normalization, Python, SQL  
**Why it matters:** Multi-source data integration is the bread and butter of airline DE work  

---

### 🔴 Hard Projects (Stretch Goals)

---

#### 🔴 #37 · Fraud Detection — Real-Time Event Pipeline
**Why it's hard:** Real-time fraud detection requires a streaming architecture (Kafka or AWS Kinesis), low-latency event processing, and integration with an ML scoring service.  
**Skills gap:** Apache Kafka, Spark Streaming or Flink, real-time ML serving  

---

#### 🔴 #22 · Dynamic Pricing — Revenue Management Data Infrastructure
**Why it's hard:** Revenue management systems process millions of price requests per day. The data infrastructure must be extremely low-latency and handle high-throughput writes.  
**Skills gap:** High-throughput streaming, OLAP databases (ClickHouse, Druid), real-time feature engineering  

---

#### 🔴 #40 · Digital Transformation — Enterprise Data Architecture Design
**Why it's hard:** This requires designing an enterprise-scale data platform (data mesh, data lakehouse, or data warehouse) for a complex multi-system airline environment.  
**Skills gap:** Data mesh concepts, cloud architecture (AWS/GCP), data governance, enterprise integration patterns  

---

### ⭐ Top 5 Portfolio Projects for Data Engineers

---

#### ⭐ Portfolio Project 1: Airline OTP Data Pipeline with Airflow + dbt
**Based on Analysis #15**

**What to build:** A fully automated data pipeline that ingests BTS monthly OTP data, transforms it with dbt, and loads it into a PostgreSQL warehouse. Orchestrate with Apache Airflow. Include data quality tests.

**Tech stack:** Python · Apache Airflow · dbt · PostgreSQL · Docker  
**Deliverables:**
- GitHub repo with Airflow DAGs, dbt models, and schema documentation
- dbt tests for data quality (not-null checks, accepted values, relationships)
- README with architecture diagram and how to run locally with Docker Compose

**Skills demonstrated:** Orchestration (Airflow), transformation (dbt), pipeline design, data quality  
**Why it impresses:** Using the same data sources that real airline analysts use (BTS) shows domain awareness. The dbt + Airflow combination is the modern standard DE stack.  

---

#### ⭐ Portfolio Project 2: Route Profitability Dimensional Model (Star Schema)
**Based on Analysis #3**

**What to build:** Design and implement a star schema for airline route profitability. Use BTS data as your source. Build dbt models for staging, intermediate, and mart layers. Document with dbt docs.

**Tech stack:** Python · dbt · PostgreSQL or BigQuery · SQL  
**Deliverables:**
- Complete dbt project with staging → intermediate → mart layers
- `fct_route_profitability` fact table with dimension tables for routes, carriers, airports, dates
- Auto-generated dbt documentation site

**Skills demonstrated:** Dimensional modeling, dbt layered architecture, SQL, data documentation  
**Why it impresses:** Dimensional modeling is the most common topic in DE interviews. A published dbt project with good documentation stands out immediately.  

---

#### ⭐ Portfolio Project 3: Loyalty Program SCD Type 2 Pipeline
**Based on Analysis #29**

**What to build:** Build a pipeline that simulates loyalty member tier changes over time using SCD Type 2, enabling accurate point-in-time queries on member status and cohort retention analysis.

**Tech stack:** Python · dbt Snapshots · PostgreSQL · pandas  
**Deliverables:**
- Python script to generate realistic synthetic loyalty member data with tier changes
- dbt Snapshot implementing SCD Type 2 for member tier history
- SQL cohort retention query with results exported as CSV

**Skills demonstrated:** SCD Type 2 (classic DE interview topic), dbt Snapshots, slowly changing data  
**Why it impresses:** SCD Type 2 is asked in almost every data engineering interview. Having a real, working example is a significant differentiator.  

---

#### ⭐ Portfolio Project 4: Fuel Efficiency & Emissions Data Pipeline
**Based on Analysis #10 + #30**

**What to build:** A pipeline that ingests aircraft fuel consumption data (or a synthetic dataset), joins to ICAO emission factors, computes CO₂ per ASK per aircraft type, and loads to a dashboard-ready table. Schedule with Airflow.

**Tech stack:** Python · Airflow · PostgreSQL · pandas  
**Deliverables:**
- Airflow DAG for scheduled monthly refresh
- Python transform script with data quality checks
- Output table ready for BI tool connection

**Skills demonstrated:** Pipeline orchestration, data quality, external data source integration, automation  
**Why it impresses:** ESG data pipelines are a growing area. Demonstrates awareness of regulatory data requirements.  

---

#### ⭐ Portfolio Project 5: Multi-Source Airline Data Integration (MRO + Flight Ops)
**Based on Analysis #14**

**What to build:** Simulate two source systems (MRO maintenance records + flight operations schedule) in CSV/JSON format. Build a Python pipeline that ingests both, reconciles on `aircraft_id`, flags data quality issues, and loads to a unified maintenance + utilization fact table.

**Tech stack:** Python · pandas · SQLAlchemy · PostgreSQL · Great Expectations  
**Deliverables:**
- Synthetic data generators for both source systems (run-able scripts)
- Python ETL pipeline with reconciliation and quality checks using Great Expectations
- Output schema with documentation

**Skills demonstrated:** Multi-source integration, data reconciliation, data quality frameworks  
**Why it impresses:** Multi-system data integration is the #1 challenge in airline data engineering. Showing you understand the complexity (and can solve it) is a strong signal.  

---

## 🟢 Data Scientist — Project Rankings

> **Your goal as a DS:** Build predictive models, optimization algorithms, and statistical analyses that generate forward-looking insights. Your SQL is for data extraction; Python is for modeling (scikit-learn, statsmodels, XGBoost). Focus on projects with clear prediction targets, measurable business outcomes, and interpretable results.

---

### 🟢 Easy Projects (Start Here)

---

#### 🟢 #4 · Seasonal Demand Forecasting
**Why it's easy for DS:** Time series forecasting with clear seasonality. A great starter ML project — use Facebook Prophet or ARIMA on monthly passenger data.  
**What you build:** A demand forecast model for 1–2 routes, 6–12 months ahead, with confidence intervals  
**Python skills used:** pandas, Facebook Prophet or statsmodels ARIMA, matplotlib for forecast visualization  
**Target variable:** Monthly passengers (or RPK) per route  
**Why it matters:** Demand forecasting is the most fundamental data science problem in aviation  

---

#### 🟢 #15 · On-Time Performance — Delay Prediction (Basic Classification)
**Why it's easy for DS:** Binary classification (delayed vs. on-time) with interpretable features (route, carrier, time of day, month). A classic introductory ML problem.  
**What you build:** A logistic regression or decision tree classifier predicting whether a flight will be delayed, trained on BTS historical data  
**Python skills used:** pandas, scikit-learn (LogisticRegression, DecisionTreeClassifier), confusion matrix, feature importance  
**Target variable:** `is_delayed` (binary: departure delay > 15 min)  
**Why it matters:** Delay prediction is a real operational use case. Airlines use this for proactive rebooking and crew management.  

---

#### 🟢 #25 · Passenger Yield Regression Model
**Why it's easy for DS:** Predicting yield (revenue / RPK) is a regression problem with interpretable features. Clear target variable, available data.  
**What you build:** A regression model predicting passenger yield given route, season, cabin class, and booking lead time  
**Python skills used:** pandas, scikit-learn LinearRegression, Ridge/Lasso, feature engineering, cross-validation  
**Target variable:** `yield` (revenue per RPK)  
**Why it matters:** Demonstrates understanding of the commercial side of aviation  

---

#### 🟢 #30 · Emissions Forecasting Model
**Why it's easy for DS:** Emissions are a direct function of fuel consumption. Regression modeling with clear inputs and outputs.  
**What you build:** A regression model predicting CO₂ emissions per flight given aircraft type, route distance, and load factor  
**Python skills used:** pandas, scikit-learn, polynomial regression, matplotlib residual plots  
**Target variable:** `co2_kg` per flight  

---

#### 🟢 #27 · Loyalty Program Breakage Prediction
**Why it's easy for DS:** Predicting whether a member will redeem their points is a binary classification problem with rich behavioral features.  
**What you build:** A classifier predicting the probability that a loyalty member will redeem points in the next 6 months  
**Python skills used:** pandas, scikit-learn (LogisticRegression, RandomForest), ROC curve, SHAP for interpretability  
**Target variable:** `will_redeem` (binary)  

---

### 🟡 Medium Projects (Build Momentum)

---

#### 🟡 #11 · Aircraft Maintenance — Predictive Maintenance Model
**Why it's medium:** Predicting component failure before it happens (binary classification). Requires feature engineering from maintenance logs and flight cycle data.  
**What you build:** A model predicting the probability of an unplanned maintenance event within the next 30 days for a given aircraft  
**Python skills used:** pandas, scikit-learn (RandomForest, XGBoost), class imbalance handling (SMOTE), SHAP  
**Target variable:** `unplanned_maintenance_next_30d` (binary)  
**Why it matters:** Predictive maintenance is a top-5 use case for ML in aviation  

---

#### 🟡 #29 · Customer Churn Prediction (Loyalty Program)
**Why it's medium:** Churn prediction uses survival analysis or standard classification. Requires cohort construction and time-based feature engineering.  
**What you build:** A model predicting which loyalty members are at risk of churning (no activity in 6+ months)  
**Python skills used:** pandas, scikit-learn, survival analysis (lifelines library), SHAP  
**Target variable:** `churned_90d` (binary)  
**Why it matters:** Loyalty churn prediction directly drives retention marketing spend  

---

#### 🟡 #13 · Load Factor Forecasting (Time Series + ML)
**Why it's medium:** Combines time series decomposition with feature-rich ML models. Requires careful feature engineering (lag features, seasonality indicators, competitor data).  
**What you build:** A load factor prediction model for 1–3 months ahead by route, comparing ARIMA vs. XGBoost with lag features  
**Python skills used:** pandas, statsmodels, scikit-learn, XGBoost, cross-validation with time series split  
**Target variable:** `monthly_load_factor` per route  

---

#### 🟡 #3 · Route Market Share Prediction
**Why it's medium:** Predicting market share changes requires competitor feature engineering. Multi-class classification or regression with business implications.  
**What you build:** A model predicting whether a route's market share will increase, decrease, or stay flat next quarter  
**Python skills used:** pandas, scikit-learn, feature engineering (price diff vs. competitors, frequency ratio), model evaluation  
**Target variable:** Market share direction (classification) or market share % (regression)  

---

#### 🟡 #5 · Route Launch Feasibility — Demand Estimation Model
**Why it's medium:** Estimating demand for a new route (no historical data) requires a gravity model or analogous route benchmarking. Classic transportation economics.  
**What you build:** A gravity model estimating potential passenger demand for a new O&D pair based on population, GDP, distance, and competing routes  
**Python skills used:** pandas, statsmodels OLS, gravity model formulation, cross-validation on held-out routes  
**Why it matters:** This is how airlines actually do route feasibility. Knowing the gravity model is niche and impressive.  

---

#### 🟡 #31 · De-icing Cost Prediction (Weather-Driven Regression)
**Why it's medium:** Integrating weather forecast data with historical cost data. Time-series regression with external regressors.  
**What you build:** A model predicting de-icing event frequency and cost per airport per month using weather variables  
**Python skills used:** pandas, scikit-learn, Prophet with regressors, matplotlib  
**Target variable:** `deicing_events_per_month`, `deicing_cost_per_month`  

---

#### 🟡 #24 · Cargo Revenue Optimization Model
**Why it's medium:** Cargo capacity allocation (weight, volume, yield class) is a multi-constraint optimization problem — simpler than passenger revenue management but a good introduction.  
**What you build:** A linear programming model that allocates cargo capacity to maximize revenue given weight and volume constraints  
**Python skills used:** pandas, scipy.optimize or PuLP for linear programming  
**Why it matters:** Optimization (LP/ILP) is a core DS skill that analysts rarely demonstrate  

---

#### 🟡 #33 · Fuel Price Forecasting and Hedging Simulation
**Why it's medium:** Time series forecasting of fuel prices + Monte Carlo simulation to evaluate hedging strategies.  
**What you build:** A fuel price forecast model + a Monte Carlo simulation comparing P&L outcomes under different hedge ratios  
**Python skills used:** pandas, statsmodels ARIMA, numpy for Monte Carlo simulation, matplotlib for scenario distributions  
**Why it matters:** Quantitative risk modeling is rare in junior DS portfolios — an instant differentiator  

---

### 🔴 Hard Projects (Stretch Goals)

---

#### 🔴 #1 · Route Network Optimization
**Why it's hard:** True network optimization is a graph problem with thousands of nodes and arcs. Requires operations research techniques (integer programming, graph algorithms).  
**Skills gap:** NetworkX, integer programming (Gurobi/OR-Tools), large-scale optimization  

---

#### 🔴 #22 · Dynamic Pricing Model (Revenue Management)
**Why it's hard:** Building a working revenue management system requires demand modeling, price elasticity estimation, seat inventory control, and competitive response modeling.  
**Skills gap:** Revenue management theory (EMSR algorithms, nested booking limits), Markov Decision Processes, online learning  

---

#### 🔴 #17 · Crew Scheduling Optimization
**Why it's hard:** Crew scheduling is an NP-hard combinatorial optimization problem. Industrial-strength solvers (Gurobi, CPLEX) are typically required.  
**Skills gap:** Combinatorial optimization, constraint programming, column generation  

---

#### 🔴 #37 · Fraud Detection with Real-Time ML
**Why it's hard:** Requires a real-time ML inference system with low latency. Model performance must be monitored continuously with concept drift detection.  
**Skills gap:** MLflow, model serving (FastAPI + Docker), concept drift detection, imbalanced classification at scale  

---

#### 🔴 #39 · Alliance Revenue Synergy Measurement (Causal Inference)
**Why it's hard:** Measuring the *causal* revenue impact of alliance membership (not just correlation) requires quasi-experimental methods (difference-in-differences, synthetic control).  
**Skills gap:** Causal inference (DiD, synthetic control), econometrics, DoWhy library  

---

### ⭐ Top 5 Portfolio Projects for Data Scientists

---

#### ⭐ Portfolio Project 1: Flight Delay Prediction — End-to-End ML Project
**Based on Analysis #15**

**What to build:** A complete ML pipeline: data ingestion from BTS → feature engineering → model training → evaluation → explainability with SHAP. Compare at least 3 models (logistic regression, random forest, XGBoost) with proper cross-validation.

**Tech stack:** Python · pandas · scikit-learn · XGBoost · SHAP · matplotlib  
**Deliverables:**
- Jupyter Notebook with full pipeline (data → features → model → evaluation)
- SHAP plots explaining which features drive delays
- Deployed model as a simple Flask/Streamlit app (bonus)

**Skills demonstrated:** Classification, model comparison, cross-validation, model explainability (SHAP)  
**Why it impresses:** Uses real aviation data. SHAP explanations show you understand model interpretability — critical for airlines who need to explain decisions to operations teams.  
**Dataset:** [BTS On-Time Performance](https://www.transtats.bts.gov/)  

---

#### ⭐ Portfolio Project 2: Predictive Maintenance — Aircraft AOG Risk Model
**Based on Analysis #11**

**What to build:** Using a synthetic or public maintenance dataset, build a model predicting unplanned maintenance risk. Focus on handling class imbalance (unplanned events are rare) and making predictions interpretable.

**Tech stack:** Python · pandas · scikit-learn · XGBoost · SMOTE · SHAP  
**Deliverables:**
- Feature engineering notebook (rolling averages of flight cycles, time-since-last-check, aircraft age)
- Model comparison (logistic regression vs. random forest vs. XGBoost)
- SHAP beeswarm plot showing top risk factors
- Business quantification: "If we flag top 10% risk aircraft for inspection, we prevent X% of AOG events"

**Skills demonstrated:** Class imbalance handling, feature engineering from time-series maintenance logs, SHAP  
**Why it impresses:** Predictive maintenance is one of the most valuable ML use cases in aviation. Quantifying the business impact (prevented AOG events) transforms it from a technical exercise into a business story.  

---

#### ⭐ Portfolio Project 3: Airline Passenger Demand Forecasting
**Based on Analysis #4 + #5**

**What to build:** A demand forecasting model for 5–10 U.S. routes. Compare classical time series (ARIMA, Prophet) vs. ML approaches (XGBoost with lag features). Include external regressors (fuel prices, GDP, holiday calendar).

**Tech stack:** Python · pandas · Facebook Prophet · statsmodels · XGBoost · matplotlib  
**Deliverables:**
- Forecasting notebook comparing ARIMA vs. Prophet vs. XGBoost
- Evaluation metrics: MAE, MAPE, coverage of prediction intervals
- Visualization of forecasts with confidence bands for 3–6 months ahead

**Skills demonstrated:** Time series forecasting, model selection, external regressor handling, forecast evaluation  
**Why it impresses:** Demand forecasting is the single most common DS job description in aviation. A clean, well-evaluated forecasting project directly answers the question "can you build models we'd actually use?"  

---

#### ⭐ Portfolio Project 4: Loyalty Member Churn Prediction + SHAP Explainability
**Based on Analysis #29 + #27**

**What to build:** Build a churn prediction model for a loyalty program (use synthetic data you generate or airline loyalty disclosures). Focus heavily on SHAP explainability to make actionable recommendations.

**Tech stack:** Python · pandas · scikit-learn · XGBoost · SHAP · Streamlit  
**Deliverables:**
- Synthetic data generation script with realistic behavioral patterns
- Churn prediction model with proper train/validation/test split
- SHAP summary plot + force plots for individual member predictions
- Streamlit app where you can enter a member profile and see their churn probability + top risk factors

**Skills demonstrated:** Binary classification, model explainability, interactive ML apps  
**Why it impresses:** The Streamlit app turns your model into something anyone can interact with — a huge differentiator in portfolio presentations. SHAP explains *why* someone is at risk, which is what retention teams actually need.  

---

#### ⭐ Portfolio Project 5: Fuel Hedging Monte Carlo Simulation
**Based on Analysis #33 + #36**

**What to build:** Build a fuel price forecasting model (ARIMA on crude oil prices) and run a Monte Carlo simulation to compare the P&L distribution across different hedging strategies (0%, 25%, 50%, 75%, 100% hedged).

**Tech stack:** Python · pandas · statsmodels · numpy · matplotlib  
**Deliverables:**
- Fuel price forecast model (ARIMA or Prophet) with 12-month horizon
- Monte Carlo simulation (5,000+ scenarios) generating P&L distribution per hedge ratio
- Visualization: overlapping P&L distributions per strategy, VaR (Value at Risk) comparison table
- Business recommendation: "At the 95th percentile of fuel price scenarios, a 50% hedge saves $X vs. unhedged"

**Skills demonstrated:** Time series forecasting, Monte Carlo simulation, financial risk quantification  
**Why it impresses:** Almost no junior DS portfolios include quantitative risk analysis. This project alone signals you understand both aviation economics and statistical modeling — a rare combination. The "VaR comparison" shows financial analysis sophistication.  

---

## Master Comparison Table — All 40 Projects

| # | Analysis Name | DA Ease | DE Ease | DS Ease | DA Portfolio | DE Portfolio | DS Portfolio |
|---|---|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | Route Network and Hub Optimization | 🔴 | 🔴 | 🔴 | — | — | — |
| 2 | Hub Connectivity and Spoke Development | 🟡 | 🟡 | 🟡 | — | — | — |
| 3 | Route Profitability and Market Share | 🟢 | 🟡 | 🟡 | ⭐ | ⭐ | — |
| 4 | Seasonal Demand and Network Flexibility | 🟢 | 🟡 | 🟢 | ⭐ | — | ⭐ |
| 5 | Market Entry and Route Launch Feasibility | 🟡 | 🟡 | 🟡 | — | — | — |
| 6 | Competitor Route Overlap | 🟡 | 🟡 | 🟡 | — | — | — |
| 7 | Regulatory Route Rights and Open Skies | 🟢 | 🟢 | 🟢 | — | — | — |
| 8 | Fleet Utilization and Efficiency | 🟢 | 🟡 | 🟡 | — | — | — |
| 9 | Aircraft Leasing: Buy vs. Lease | 🟡 | 🟡 | 🔴 | — | — | — |
| 10 | Fuel Efficiency per Aircraft Type | 🟢 | 🟢 | 🟡 | — | ⭐ | — |
| 11 | Aircraft Maintenance Planning & Downtime | 🟢 | 🟡 | 🟡 | — | — | ⭐ |
| 12 | Pilot Training & Simulator Utilization | 🟢 | 🟢 | 🟢 | — | — | — |
| 13 | Load Factor and Capacity Management | 🟢 | 🟡 | 🟡 | ⭐ | ⭐ | — |
| 14 | MRO Cost Analysis | 🟢 | 🟡 | 🟡 | — | ⭐ | — |
| 15 | On-Time Performance and Reliability | 🟢 | 🟡 | 🟢 | ⭐ | ⭐ | ⭐ |
| 16 | Airport Resource Optimization | 🟡 | 🟡 | 🟡 | — | — | — |
| 17 | Crew Scheduling and Labor Cost | 🟡 | 🟡 | 🔴 | — | — | — |
| 18 | Cabin Configuration and Seat Density | 🟡 | 🟡 | 🟡 | — | — | — |
| 19 | Ground Operations Efficiency | 🟢 | 🟡 | 🟡 | — | — | — |
| 20 | Airport and Ground Handling Cost | 🟡 | 🟡 | 🟡 | — | — | — |
| 21 | Passenger Flow and Boarding Efficiency | 🟢 | 🟡 | 🟡 | — | — | — |
| 22 | Core Services Revenue & Dynamic Pricing | 🟡 | 🔴 | 🔴 | — | — | — |
| 23 | Ancillary Revenue and Yield Management | 🟡 | 🟡 | 🟡 | — | — | — |
| 24 | Cargo Revenue and Capacity Utilization | 🟡 | 🟡 | 🟡 | — | — | — |
| 25 | Passenger Yield and Demographic Analysis | 🟢 | 🟡 | 🟢 | ⭐ | — | — |
| 26 | In-Flight Service and Product Differentiation | 🟢 | 🟢 | 🟢 | — | — | — |
| 27 | Loyalty Program Redemption & Breakage Rate | 🟢 | 🟡 | 🟢 | ⭐ | — | — |
| 28 | Passenger Experience Differentiation | 🟡 | 🟡 | 🟡 | — | — | — |
| 29 | Customer Satisfaction of Loyalty Programs | 🟡 | 🟡 | 🟡 | — | ⭐ | ⭐ |
| 30 | Environmental Compliance & Sustainability | 🟢 | 🟡 | 🟢 | ⭐ | ⭐ | — |
| 31 | De-icing and Weather Contingency Cost | 🟢 | 🟡 | 🟡 | — | — | — |
| 32 | Safety and Incident Reporting Compliance | 🟢 | 🟢 | 🟢 | — | — | — |
| 33 | Fuel Cost and Hedging Strategy | 🟡 | 🟡 | 🟡 | — | — | ⭐ |
| 34 | Debt Structure and Lease Obligations Review | 🔴 | 🟡 | 🔴 | — | — | — |
| 35 | Airport and Route-Level Cost Structure | 🟢 | 🟡 | 🟡 | — | — | — |
| 36 | Fuel Tankering Strategy | 🟡 | 🟡 | 🟡 | — | — | — |
| 37 | Revenue Protection and Fraud Detection | 🟡 | 🔴 | 🔴 | — | — | — |
| 38 | Alliance and Codeshare Evaluation | 🟡 | 🟡 | 🟡 | — | — | — |
| 39 | Alliance Contribution and Revenue Synergy | 🟡 | 🟡 | 🔴 | — | — | — |
| 40 | IT and Digital Transformation Assessment | 🔴 | 🔴 | 🔴 | — | — | — |

---

## Public Datasets to Build Your Portfolio

You don't need to work at an airline to build an airline portfolio. These free public datasets cover most of the analyses above.

| Dataset | Source | Covers | Best For |
|---|---|---|---|
| **On-Time Performance** | [BTS](https://www.transtats.bts.gov/OT_Delay/OT_DelayCause1.asp) | Delays, OTP, routes, carriers | DA #15 · DS #15 |
| **T-100 Domestic Segment** | [BTS](https://www.transtats.bts.gov/) | ASM, RPM, passengers, load factor | DA #3, #13 · DE #3, #13 |
| **DB1B Origin-Destination Fare** | [BTS](https://www.transtats.bts.gov/DatabaseInfo.asp?QO_VQ=EFD) | Average fares by O&D pair | DA #3, #6 · DS #25 |
| **Form 41 Financial Data** | [BTS](https://www.transtats.bts.gov/databases.asp) | Airline revenue, cost, fuel expenses | DA #3, #35 · DS #33 |
| **Open Flights Database** | [openflights.org](https://openflights.org/data.html) | Airports, routes, airline metadata | All route analyses |
| **Aviation Weather (METAR)** | [NOAA ASOS](https://www.ncei.noaa.gov/products/land-based-station/automated-surface-weather-observations) | Weather conditions by airport | DA #31 · DS #31 |
| **EIA Jet Fuel Prices** | [EIA](https://www.eia.gov/dnav/pet/pet_pri_spt_s1_d.htm) | Daily/monthly jet fuel prices | DA/DS #33, #36 |
| **EUROCONTROL Data** | [EUROCONTROL](https://www.eurocontrol.int/dashboard/rnd-data-archive) | European flight data, delays, emissions | All for European aviation |
| **ICAO Environmental Report** | [ICAO](https://www.icao.int/environmental-protection) | Emissions factors, sustainability KPIs | DA #30 |
| **Airline Quality Rating** | [AQR](http://www.airlinequalityrating.com/) | Customer satisfaction, complaints, OTP | DA #28, #29 |

---

## Suggested Learning Path by Role

### 🔵 If you want to be a Data Analyst

**Month 1–2 (Domain + Foundations):**
- Learn aviation KPIs: RPK, ASK, load factor, yield, CASK — read the IATA Economics Briefing
- Complete projects #15 and #13 using BTS data as learning exercises
- Build your first Tableau Public or Power BI dashboard from BTS OTP data

**Month 3–4 (Portfolio Building):**
- Build Portfolio Projects 1 and 2 (OTP Dashboard + Route Profitability)
- Practice SQL window functions: `RANK()`, `LAG()`, `DATE_TRUNC()` on the BTS datasets

**Month 5–6 (Differentiation):**
- Build Portfolio Project 3 (Sustainability) — differentiates from other candidates
- Learn basic dbt to show you can work with modern analytics engineering tools
- Target: Apply for junior/analyst positions at airlines, airport operators, and aviation consultancies

---

### 🟠 If you want to be a Data Engineer

**Month 1–2 (Foundation Stack):**
- Learn Apache Airflow (take the Astronomer Academy free course)
- Learn dbt Core (free dbt Learn courses)
- Set up a local PostgreSQL + dbt + Airflow environment with Docker Compose

**Month 3–4 (Portfolio Building):**
- Build Portfolio Projects 1 (Airflow + dbt OTP pipeline) and 2 (Star Schema)
- Practice dimensional modeling: read *The Data Warehouse Toolkit* (Kimball) — at least Ch. 1–3

**Month 5–6 (Differentiation):**
- Build Portfolio Project 3 (SCD Type 2 Loyalty Pipeline)
- Learn Great Expectations or dbt tests for data quality
- Target: Apply to data engineering roles at airlines, GDSs (Amadeus, Sabre), or aviation tech companies

---

### 🟢 If you want to be a Data Scientist

**Month 1–2 (ML Foundations + Domain):**
- Complete Andrew Ng's ML Specialization (Coursera) if not already done
- Read about airline revenue management: *The Practice of Revenue Management* (free academic resources available)
- Complete projects #15 (delay prediction) and #4 (demand forecasting) as learning exercises

**Month 3–4 (Portfolio Building):**
- Build Portfolio Projects 1 (Flight Delay ML) and 3 (Demand Forecasting)
- Learn SHAP for model explainability — critical in regulated aviation environments
- Learn Prophet and ARIMA for time series

**Month 5–6 (Differentiation):**
- Build Portfolio Project 5 (Fuel Hedging Monte Carlo) — the rarest project type for a junior DS
- Learn the basics of linear programming (PuLP) for optimization problems
- Target: Apply to data science roles at airlines, MRO providers, and aviation analytics startups

---

## Interview Talking Points by Project

Use these when an interviewer asks *"Tell me about a project you've worked on."*

---

**For Project #15 (On-Time Performance):**
> *"I built an analysis of U.S. domestic flight delays using BTS data. I found that [carrier X] had the highest delay propagation — a delay in the morning creates a cascade through the day. I used SQL window functions to calculate delay cascades and visualized the spread in Python. The project taught me how operational data in aviation is highly interconnected and why upstream delays matter so much."*

---

**For Project #13 (Load Factor):**
> *"I analyzed seasonal load factor patterns across 20+ routes using BTS T-100 data. I identified three routes that were operating at 60% load factor in Q1 but 90%+ in Q3 — a sign of undersized winter capacity. I quantified the revenue opportunity if they matched their Q3 load factor year-round, which turned out to be a significant number. This taught me how to translate an operational metric into a business impact number."*

---

**For Predictive Maintenance (DS #11):**
> *"I built a predictive model to flag aircraft at high risk of unplanned maintenance events. The key challenge was class imbalance — unplanned events are rare — so I used SMOTE to oversample the minority class. I also added SHAP explanations so the model could tell a maintenance crew not just that an aircraft is high-risk, but specifically which factors (e.g., high flight cycles since last heavy check) are driving that prediction."*

---

**For dbt + Airflow Pipeline (DE #1):**
> *"I built a complete data pipeline using Apache Airflow and dbt on BTS on-time performance data. The Airflow DAG runs monthly to ingest new data, dbt handles the transformations through staging, intermediate, and mart layers, and the output feeds a Power BI dashboard. I also added dbt tests for data quality — not-null checks, value range validation, referential integrity — so the pipeline fails loud if the source data has issues."*

---

*Built from the framework in: "How to Analyze an Airline Company" · Will Bachman · Umbrex (2024)*  
*Public data sources: U.S. Bureau of Transportation Statistics · ICAO · EIA · EUROCONTROL*
