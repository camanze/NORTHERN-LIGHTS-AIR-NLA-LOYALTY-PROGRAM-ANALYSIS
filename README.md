# NORTHERN LIGHTS AIR (NLA) LOYALTY PROGRAM ANALYSIS

**OBJECTIVE:**

In an effort to boost loyalty program enrolment and enhance customer engagement, NLA ran a promotional campaign between February and April 2018. This report analyzes the campaign’s effectiveness in two dashboards: Flight Activity and Loyalty History. The analysis evaluates enrolment trends, flight activity, and demographic segmentation, providing insights into the campaign’s overall impact and success.

**DATASET DESCRIPTION:**

The dataset used for this project was sourced from Maven Analytics and can be found [here](https://mavenanalytics.io/data-playground?order=date_added%2Cdesc&search=loyalty)
The folder contains 4 tables (Airline Loyalty Data Dictionary, Calendar, Customer Flight Activity, and Customer Loyalty History), bearing 412,230 records of the airline's customers' activities between 2017 and 2018. The dataset is almost clean from source, and I had to do minimal cleaning before using them for the project.

For the purpose of this project, I used only 2 of the tables: Customer Flight Activity and Customer Loyalty History. These 2 key tables have all the information we need for the analysis.

**ANALYTIC TOOLS USED**

**EXCEL:** 
* I used MS Excel to clean and get the dataset ready.
* Added a 'Date' column to both tables using the Date function in excel.
  
**POWER BI:** This is where most of the data transformation happened.
* Added new column to help with the project analysis; 'Period' - used to distinguish customer enrolments before, during and after the promotional campaign.
* Transformed data type for the column 'Dollar Cost Point Redeemed' to Currency ($ CAD), for for proper analysis.
* Vizualized some Measures using DAX (eg, Customers Enroled, Average Monthly Flights, Standard Enrolments, 2018 Promotion Enrolments, Average Monthly Enrolments, Total Cancellations, Total Points Accumulated, and Total Points Redeemed)
