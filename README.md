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

<img width="915" height="431" alt="Total Expenditure Over Time" src="https://github.com/user-attachments/assets/74844663-5d4f-4ab2-8613-0a962a8d0b76" />
<img width="876" height="426" alt="Filtered Year View" src="https://github.com/user-attachments/assets/485515e4-12f4-439c-a185-c71e2b515ddc" />

<img width="1458" height="730" alt="Interactive Slicer Demo GIF" src="https://github.com/user-attachments/assets/6e136190-abd6-4b93-b595-44eaa95bcdaa" />

**How it was built & how it works:**
* **Interactive Navigation:** The GIF above demonstrates how stakeholders can seamlessly toggle between a high-level, multi-year overview and granular single-year views using an interactive **Year Slicer**.
* **Data & Schema Transformation:** To ensure accurate chronological tracking, the raw dataset schema was cleaned in Power Query—specifically standardizing date formats so time-series trends render in proper sequential order without sorting errors.


What was found was that 

### Question 2:  What percentage of total spend goes to local vendors compared to non-local suppliers?

To answer this question what was done was the use of the moddeling tool combinded with sql queries spcfically to select the avg via dividing by sums of totals in tables this data was then further transformed by the slicer used above allow for representation of this information through each year to see exaclty how this information was cahnged. 

What was found was that 


### Question 3:  Indigenous Procurement Growth 

To answer this question the method was the same as question two but the query tiself was more targeted 

This resulted in viding out that ....



## Data Source  
Townsville City Council. (2026). Townsville City Council value of local spend (purchase orders) [Data set]. In Data.gov.au. https://data.gov.au/data/dataset/townsville-city-council-value-of-local-spend

## Technical Implementation & Skills Demonstrated
