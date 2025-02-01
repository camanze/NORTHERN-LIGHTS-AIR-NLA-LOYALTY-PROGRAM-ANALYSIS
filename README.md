# NORTHERN LIGHTS AIR (NLA) LOYALTY PROGRAM ANALYSIS

**OBJECTIVE:**

In an effort to boost loyalty program enrolment and enhance customer engagement, NLA ran a promotional campaign between February and April 2018. This report analyzes the campaign’s effectiveness in two dashboards: Flight Activity and Loyalty History. The analysis evaluates enrolment trends, flight activity, and demographic segmentation, providing insights into the campaign’s overall impact and success.

**DATA DESCRIPTION AND COLLECTION:**

The dataset used for this project was sourced from Maven Analytics and can be found [here](https://mavenanalytics.io/data-playground?order=date_added%2Cdesc&search=loyalty)
The folder contains 4 tables (Airline Loyalty Data Dictionary, Calendar, Customer Flight Activity, and Customer Loyalty History), bearing 412,230 records of the airline's customers' activities between 2017 and 2018. The dataset is almost clean from source, and I had to do minimal cleaning before using them for the project.

For the purpose of this project, I used only 2 of the tables: Customer Flight Activity and Customer Loyalty History. These 2 key tables have all the information we need for the analysis.

**DATA CLEANING AND PREPARATION**

**MICROSOFT EXCEL:** This was the least used tool in the course of this project. Microsoft Excel was used at the start of the project to provide an understanding of the data structure, and to provide a guide on the steps to be carried out in transforming the data using the Power Query Editor. 
* I used MS Excel to clean and get the dataset ready.
* Added a 'Date' column to both tables using the Date function in excel.
  
**POWER QUERY EDITOR:** This is where most of the data transformation happened. This is an advanced feature of Power BI that allows transformation and cleaning to be carried out on a dataset.
* Added new column to help with the project analysis; 'Period' - used to distinguish customer enrolments before, during and after the promotional campaign.
* Transformed data type for the column 'Dollar Cost Point Redeemed' to Currency ($ CAD), for for proper analysis.
* Vizualized some Measures using DAX (eg, Customers Enroled, Average Monthly Flights, Standard Enrolments, 2018 Promotion Enrolments, Average Monthly Enrolments, Total Cancellations, Total Points Accumulated, and Total Points Redeemed).


**ANALYSIS AND VISUALIZATION USING POWER BI**

After completing the data cleaning and preparation process, I proceeded with the analysis and visualization stages. To enhance navigation and provide a clear understanding of the project, I structured the visualizations into two distinct dashboards. These dashboards serve as an effective tool for presenting key insights derived from the analysis.

Below is a summary of the key insights from the data visualizations: 

**FLIGHT ACTIVITY:** The Flight Activity Dashboard presents key insights into customer enrollment, flight activity, points accumulation, and monthly trends, providing an overview of performance and trends before, during, and after a promotional period.
* **Customer Enrollment:** The total number of customers enrolled in the program reached 16,737, with the majority (15,766) opting for standard enrollment. A total of 971 enrollments were recorded during the 2018 promotional period, indicating a slight uptick in engagement due to the promotion.
*  **Flight Activity:** Overall, 509,000 flights were completed, with an average of 4,240 flights per month. This data underscores consistent flight activity throughout the reporting period, with particular attention to fluctuations surrounding the promotional period.
*  **Points Accumulation:** Before the promotion, a total of 354,308,847 points were accumulated. During the promotional period, this figure rose significantly, with 75,316,895.5 additional points accrued. After the promotion, the total points accumulated stood at 366,923,250. Notably, the points accumulation surged during the promotion and continued to remain high post-promotion, reflecting the impact of the initiative on customer activity.
*  **Average Monthly Flights:** The average number of monthly flights demonstrated a noticeable change across the three periods. Prior to the promotion, the average was 19,715.58 flights per month. During the promotion, this number dropped to 4,086, likely due to a temporary reduction in activity while customers focused on accumulating points. However, after the promotion, the average monthly flights rebounded to 18,599.08, showing a return to pre-promotion flight volumes.
*  **Average Flight Distance:** In terms of flight distances, there was a marked increase after the promotion. Prior to the promotion, the average flight distance was 1,711.43 kilometers. This decreased to 1,452.84 kilometers during the promotion, possibly indicating shorter flights or adjustments in customer behavior during the promotion period. After the promotion, the average flight distance jumped significantly to 2,476.85 kilometers, suggesting a shift back to longer flights as customer engagement returned to normal levels.
*  **Monthly Flight Volumes (2017 vs. 2018):** A comparison of monthly flight volumes between 2017 and 2018 highlights substantial growth in 2018, particularly during the summer months. For example, in May 2017, 18,690 flights were recorded, while May 2018 saw an increase to 27,345. Similarly, in June 2017, there were 23,504 flights compared to 33,840 in June 2018, and similar increases were observed in July and August. These significant increases in flight activity in 2018 are a clear indicator of a positive trend in customer engagement.
*  **Dollar Cost of Points Redeemed:** The dollar cost in Canadian dollars (CAD) of points redeemed showed some fluctuations over the reporting period. Before the promotion, the cost was $5.27 per point. During the promotion, this decreased slightly to $5.14 per point. However, after the promotion, the cost rose to $6.38 per point, possibly reflecting changes in point redemption patterns or shifts in the value of the promotion itself.

![Flight Activity](https://github.com/user-attachments/assets/3dc9eb72-c6be-4bec-ba37-578af921afdd)

I added page navigation buttons on the top right end of the dashboards, to facilitate easy switching between the two dashboards.


**LOYALTY HISTORY:** The Loyalty History Dashboard provides a detailed overview of customer enrollment trends, demographics, and cancellations, offering valuable insights into the performance and reach of the loyalty program.
* **Enrollment Trends:** During the 2018 promotional period, a total of 971 new enrollments were recorded. However, the program also experienced a higher number of cancellations, with 2,067 customers opting to discontinue their membership. On average, 1,394.75 new enrollments were made per month, reflecting a steady rate of program engagement across the year.
* **Enrollment Demographics:** The dashboard also provides demographic breakdowns across various categories, offering deeper insights into the program’s reach and engagement:
1. **Gender Distribution:** Enrollment figures show a slight male-to-female split. Among standard enrollments, 660 females and 654 males joined the program. During the 2018 promotion, 41 females and 40 males enrolled, indicating a balanced interest across both genders.
2. **Loyalty Card Type:** Regarding the loyalty card types, the distribution was as follows: 600 customers enrolled in the Star card, 445 in the Nova card, and 268 in the Aurora card under the standard enrollment plan. The 2018 promotion saw 36 enrollments in the Star card, 28 in Nova, and 17 in Aurora.
3. **Education Level:** A significant portion of enrollees holds a Bachelor’s degree, with 820 standard enrollees and 53 from the promotion. College graduates made up 333 standard enrollments and 20 during the promotion. Smaller numbers were seen in other education levels, with high school graduates accounting for 61 standard and 4 promotional enrollments, while those with advanced degrees (Doctoral and Master’s) represented 59 and 41 standard enrollments, respectively, with a notable decrease in the promotional period.
4. **Marital Status:** The majority of enrollees (58.16%) are married, followed by single individuals at 26.79% and divorced individuals at 15.04%. This breakdown highlights the program’s appeal across various marital statuses.
5. **Provincial Distribution:** In terms of geographical distribution, Ontario led with the highest number of enrollments, accounting for 5,404 customers. British Columbia followed closely with 4,409 enrollments, while Quebec contributed 3,300 customers. Alberta and Manitoba had significantly smaller enrollments, with 969 and 658 customers respectively, and other provinces showed even lower numbers.


![Loyalty History](https://github.com/user-attachments/assets/b2b70e3a-0b3d-488c-81f5-f61bb1e42d57)

[Click here](https://app.powerbi.com/view?r=eyJrIjoiNmM4NzEzOTQtMmFmNi00OWExLTkxYTgtZGQ0NWVhNjRiODA3IiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9) to view the interactive Power BI design.

**CONCLUSIONS**

The Flight Activity Dashboard illustrates a dynamic period for the program, with notable increases in customer engagement, flight activity, and points accumulation, particularly during and after the promotional period. These trends suggest that the promotion was successful in driving customer participation and influencing flight patterns. The data indicates a healthy recovery in flight activity and points accumulation post-promotion, with a clear return to normal flight volumes and longer distances. 

On the other hand, the Loyalty History Dashboard provides a comprehensive view of program engagement, highlighting both opportunities and challenges. While enrollments showed steady growth, the cancellations indicate areas that may require attention in terms of customer retention. The demographic breakdown further reveals that the program attracts a well-educated and diverse group of individuals, with strong representation across multiple provinces.

Moving forward, the insights gleaned from these trends will be valuable for shaping future promotions and optimizing the customer experience. The data from these dashboards will serve as a crucial tool for refining strategies aimed at increasing enrollment, reducing cancellations, and enhancing overall program effectiveness moving forward.

**RECOMMENDATIONS**

Based on the insights from these dashboards, several key trends and areas of opportunity have emerged. Here are strategic recommendations for the airline to enhance services and optimize customer engagement moving forward:

1. **Enhance Customer Retention Programs**
 * **Address Cancellations:** With 2,067 cancellations reported in the Loyalty History Dashboard, the airline could benefit from a closer examination of the reasons behind these cancellations. Offering tailored retention strategies—such as personalized outreach, loyalty rewards, or special offers for at-risk members—could help reduce churn.
 * **Loyalty Program Optimization:** The post-promotion drop in flight activity suggests a need to adjust the loyalty program to maintain high engagement. Enhancing the rewards system, offering tiered loyalty benefits, or introducing time-limited promotions could encourage members to continue flying at the same rate after a promotion ends.

2. **Refine Promotional Strategies**
 * **Targeted Promotions Based on Demographics:** Data indicates that the program is particularly attractive to customers with bachelor’s degrees (820 enrollments in the standard program) and those in Ontario (5,404 enrollments). Future promotions could be tailored to attract more customers from other regions, as well as diverse educational backgrounds and marital statuses. Additionally, offering promotions with varied loyalty card types (Star, Nova, Aurora) could help the airline better understand which segments respond most positively.
 * **Promote Longer Flights Post-Promotion:** The increase in flight distance after the promotion (2,476.85 km) indicates that customers may be more inclined to book longer flights once the promotional period ends. Marketing campaigns could focus on longer-haul flights or destinations that offer additional value for loyal customers.

3. **Improve Engagement During the Promotion Period**
 * **Boost Enrollment During Promotions:** Although 971 new enrollments were achieved during the 2018 promotion, the drop in monthly flights (4,086 during promotion versus 19,715 before) signals a potential gap in engaging customers beyond just signing up. Introducing added incentives for those who maintain consistent flight activity during the promotion, such as bonus points or exclusive rewards, may help retain interest throughout the promotional period.
 * **Segmented Marketing Campaigns:** The loyalty data reveals different preferences across genders, education levels, and marital statuses. A more segmented approach, offering personalized promotions that speak directly to these groups, could help increase enrollment and engagement, particularly during promotional periods.

4. **Strengthen Regional Outreach**
 * **Expand in Underrepresented Provinces:** Although Ontario and British Columbia showed strong enrollment numbers, provinces such as Alberta and Manitoba demonstrated much lower engagement. Tailoring services or special promotions for customers in these areas, as well as launching regional marketing campaigns, could drive higher enrollments and flight activity.
 * **Regional Partnerships:** In addition to promotional campaigns, partnerships with local businesses or tourism organizations in underrepresented regions could help expand the airline’s customer base and strengthen regional loyalty.

5. **Optimize Flight and Distance Metrics**
 * **Increase Shorter Flights During Low Activity Periods:** The decline in average flight distance during the promotion (1,452.84 km) could be an opportunity to offer more convenient, shorter flights or regional routes. Targeting specific market segments with tailored, short-haul flight promotions could increase engagement during off-peak periods.
 * **Targeted Incentives for Long-Distance Flights:** Post-promotion, the average flight distance surged, suggesting a preference for longer routes. The airline could introduce targeted incentives for loyal customers booking longer flights, such as double points for international routes or exclusive access to certain amenities.

6. **Invest in Data-Driven Customer Insights**
  * **Use Data to Predict Flight Preferences:** By analyzing flight patterns, enrollment trends, and demographic information, the airline can predict future customer behavior and optimize flight schedules accordingly. Understanding peak travel periods and customer preferences will allow the airline to tailor its offerings, such as providing more flight options or upgrading in-demand routes.
  * **Personalized Customer Engagement:** Further leveraging customer data to personalize engagement strategies—such as offering targeted offers based on previous flight activity, preferences, and demographics—will improve customer satisfaction and loyalty.

7. **Monitor and Adjust the Cost of Points**
  * **Review Points Redemption Costs:** The rise in the dollar cost of points redeemed after the promotion ($6.38) suggests that customers may be sensitive to changes in redemption value. Ensuring that point redemption offers maintain a competitive edge and align with customer expectations will be crucial to sustaining loyalty program appeal. Offering seasonal promotions or bonuses on point redemption could further improve engagement and retention.

8. **Focus on Marketing and Education Around Loyalty Benefits**
  * **Educate Customers on Benefits of Loyalty Cards:** There is a notable difference in enrollment across loyalty card types (Star, Nova, and Aurora). This suggests that customers may need more education on the advantages of each card type. A clearer communication strategy around the different loyalty benefits could encourage customers to upgrade or switch their card types for greater rewards.
  * **Improve Awareness of Loyalty Program Benefits:** Offering new or potential customers easy-to-understand resources about loyalty program advantages (including how to maximize points and benefits) can drive interest and satisfaction.


The data from both dashboards highlight several key areas where the airline can enhance its services. By focusing on customer retention, refining promotional strategies, expanding regional outreach, and tailoring flight offerings to customer preferences, the airline can build stronger relationships with its customers. Additionally, leveraging data-driven insights to personalize offers and ensure competitive pricing for loyalty benefits will help sustain long-term customer loyalty and engagement.


