# Council-Procurement-Supplier-Diversity-Analysis-2019-2026

## Project Overview 
An interactive Power BI executive dashboard analyzing over 7 years of public procurement data. This project tracks total council expenditure, local supplier engagement, and Indigenous procurement performance to provide leadership with actionable insights into regional economic impact.


## Key Questions Tackled 

This dashboard was designed to answer three core executive questions:

- Total Spend Baseline: What is the total volume of council expenditure over time? ($2.75B total baseline across the 7-year period).

- Local Supplier Share: What percentage of total spend goes to local vendors compared to non-local suppliers? (~77.98% average local capture rate).

- Indigenous Procurement Growth: How has the share of spend dedicated to Indigenous-owned businesses trended year-over-year? (~0.97% average share).

### Question 1: What is the total volume of council expenditure over time?

To answer this, the dashboard tracks total procurement spend across the entire 2019–2026 period ($2.75B baseline) while allowing users to drill down into specific years on demand.

### Visual Comparison: Multi-Year Trends vs. Filtered Views

| Overview & Full Timeline ($2.75B Baseline) | Filtered Single-Year View (2026 Focus) |
| :---: | :---: |
| <img width="450" alt="Total Expenditure Over Time" src="https://github.com/user-attachments/assets/74844663-5d4f-4ab2-8613-0a962a8d0b76" /> | <img width="450" alt="Filtered Year View" src="https://github.com/user-attachments/assets/485515e4-12f4-439c-a185-c71e2b515ddc" /> |
| *Tracks overall multi-year council procurement expenditure.* | *Filters down dynamically using the interactive Year Slicer.* |

---

### Interactive Dashboard Demonstration

<p align="center">
  <img width="900" alt="Interactive Slicer Demo GIF" src="https://github.com/user-attachments/assets/6e136190-abd6-4b93-b595-44eaa95bcdaa" />
</p>
<p align="center"><em>Demonstrating seamless dynamic filtering across custom time horizons.</em></p>

**How it was built & how it works:**
* **Interactive Navigation:** The GIF above demonstrates how stakeholders can seamlessly toggle between a high-level, multi-year overview and granular single-year views using an interactive **Year Slicer**.
* **Data & Schema Transformation:** To ensure accurate chronological tracking, the raw dataset schema was cleaned in Power Query—specifically standardizing date formats so time-series trends render in proper sequential order without sorting errors.

### Question 2: What percentage of total spend goes to local vendors compared to non-local suppliers?

* **How it was built & how it works:**
  * **DAX & Modeling:** Created calculated measures using the `DIVIDE` function to compute exact ratios between local and non-local spend categories against the overall total baseline.
  * **Dynamic Breakdown:** Integrated a proportional **Donut Chart** tied to the year slicer, allowing stakeholders to evaluate regional capture rates across both the 7-year aggregate and individual calendar years.

* **Key Findings & Observations:**
  * **Strong Regional Retention:** Across the full 7-year timeline, total council procurement reached **$2.75B**.
  * **Local vs. Non-Local Split:** The council consistently prioritizes local vendors, retaining **77.98%** $2.14B of total spend locally, while **22.02%** $0.60B went to non-local suppliers.
  * **Cyclical Spending Patterns:** Monthly local spend fluctuates between **$11M and $55M**, showing predictable mid-year peaks (May–July) aligned with end-of-financial-year capital works.

---

### Question 3: How has the share of spend dedicated to Indigenous-owned businesses trended over time?

* **How it was built & how it works:**
  * **Targeted DAX Measures:** Developed specific percentage measures targeting Indigenous spend categories to isolate supplier diversity metrics from general procurement.
  * **Time-Series Tracking:** Placed dedicated monthly trend lines alongside multi-year summary cards to monitor baseline growth and spot specific milestone-driven contract spikes.

* **Key Findings & Observations:**
  * **Overall Baseline:** Indigenous-owned businesses accounted for an average of **0.96%** (~$0.03B) of total expenditure across the multi-year period.
  * **2022 Surge:** Drilling down into **2022** ($403.76M total spend) reveals a standout year where Indigenous procurement rose to **1.46%** ($5.9M), outperforming the multi-year average.
  * **Project-Driven Spikes:** Monthly Indigenous spend experienced sharp peaks in **May 2022 (~$1.4M)** and **July 2022 (~$1.7M)**, indicating that volume is driven by major milestone-based contract awards rather than recurring operational spend.


## Data Source  
Townsville City Council. (2026). Townsville City Council value of local spend (purchase orders) [Data set]. In Data.gov.au. https://data.gov.au/data/dataset/townsville-city-council-value-of-local-spend
