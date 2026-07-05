# Hospital-Emergency-Room-Dashboard

An interactive Power BI report built to analyze emergency room performance — tracking patient volume, wait times, satisfaction, admissions, and demographics to help hospital administrators make faster, data-driven staffing and resource decisions.


**Short Description / Purpose**

The Hospital Emergency Room Dashboard is a multi-page Power BI report that consolidates 19 months of ER visit data (April 2023 – October 2024) covering over 9,200 unique patients. It is designed to help hospital administrators, operations managers, and healthcare analysts monitor patient flow, wait times, satisfaction scores, and admission patterns, and to surface staffing and resource-allocation insights at a glance.


**Tech Stack**

The dashboard was built using the following tools and technologies:

📊 **Power BI Desktop** – Main data visualization and report-building platform.

📂 **Power Query** – Data cleaning and transformation layer for shaping raw ER records.

🧠 **DAX (Data Analysis Expressions)** – Used for measures such as Avg. Wait Time, No. of Patients, and satisfaction score aggregations.

📝 **Data Modeling** – A star-schema-style model relating the Hospital ER_Data fact table to a Date Table dimension, enabling time-based drill-downs (Year → Quarter → Month → Day) and cross-filtering across pages.

📁 **File Format** – .pbix for development.


**Data Source**

The dataset is a hospital Emergency Room records table (Hospital ER_Data) containing patient-level fields such as Patient ID, Full Name, Gender, Age, Race, Admission Date, Admission Status, Department Referral, Waittime, Waittime Status, and Satisfaction Score — paired with a supporting Date Table for time intelligence.


**Features / Highlights**

Business Problem
ER departments generate large volumes of patient data daily, but staff and administrators often lack a consolidated, visual way to spot bottlenecks. Questions like Which days and hours are busiest? Which departments receive the most referrals? Are patients being seen within acceptable wait times? are hard to answer quickly from raw records.


**Goal of the Dashboard**

To deliver an interactive reporting tool that:
Tracks core ER KPIs (patient volume, wait time, satisfaction, referrals) monthly and cumulatively.
Helps identify peak demand periods to guide staffing decisions.
Breaks down patient demographics and admission outcomes for operational and equity analysis.
Supports drill-down into individual patient-level detail when needed.


**Walkthrough of Key Visuals**

The report spans four pages:

Monthly View – KPI cards for No. of Patients, Avg. Wait Time, Patient Satisfaction Score, and No. of Patients Referred, alongside area charts trending each metric by day within a selected month. Includes a Month/Year slicer for period-over-period comparison.

Consolidated View – The same core KPIs and metrics as the Monthly View, but aggregated and charted across the full date range using column charts, giving a big-picture view of trends over the entire 19-month period.
Both views additionally include:
A Patient Admission Status pivot table and bar chart.
A clustered column chart of patients by Age Group.
A clustered bar chart of patients by Department Referral.
A donut chart showing % of patients seen within 30 minutes (Waittime Status).
A donut chart of patients by Gender, and a clustered bar chart by Patient Race.
A pivot table and column chart of patient volume by Day of Week and Admission Hour, highlighting peak traffic windows.

Patient Detail View – A detailed, filterable table listing individual patients with ID, name, gender, age, admission date hierarchy, race, wait time, department referral, and admission status — for drill-through and case-level review.

Key Takeaways – A narrative summary page distilling the analysis into plain-language insights on volume, wait times, satisfaction, referrals, peak periods, demographics, and admission patterns.


**Business Impact & Insights**

Staffing Optimization: Peak days (Mondays, Saturdays, Tuesdays) and peak hours (11 AM, 7 PM, 1 PM, 11 PM) were identified, indicating when additional staffing is most needed.
Patient Experience: Average wait time (~35.3 minutes) and average satisfaction score (4.99/10) point to clear opportunities to improve patient flow and experience.
Referral Management: General Practice and Orthopedics account for the largest share of referrals, useful for capacity planning with partner departments.
Demographic Insights: Adults aged 30–39 and 20–29 make up the largest patient segments, and admissions are nearly evenly split between admitted (4,612) and treated-and-released (4,604) patients — useful for resource and bed-capacity planning.


**Screenshots / Demos**

(https://github.com/ananyamishra1972-beep/Hospital-Emergency-Room-Dashboard/blob/main/02.%20Monthly%20View%20of%20Hospital%20Emergy%20Room.png)

(https://github.com/ananyamishra1972-beep/Hospital-Emergency-Room-Dashboard/blob/main/03.%20Consolidate%20View%20of%20H%20E%20R.png)

(https://github.com/ananyamishra1972-beep/Hospital-Emergency-Room-Dashboard/blob/main/04.%20Patient%20Detail%20View%20of%20H%20E%20R.png)

(https://github.com/ananyamishra1972-beep/Hospital-Emergency-Room-Dashboard/blob/main/05.%20Key%20Takeaways%20of%20H%20E%20R.png)
