<h1>USECASE 01 - Bank Churn Analysis</h1>

<h3>Objective</h3>
<p>To analyze and predict customer churn and risk by examining factors such as geography, gender, credit score, tenure, age, and salary. Machine learning was used to calculate the churn probability of customers. The goal is to provide actionable insights to retain customers and reduce churn.</p>

<h3>Report View</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/9b9ae585-a10c-4b93-b62e-3c8a764e4110" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/fad0cd59-c6a1-4ac5-adb4-cf8d39c9a268" style="width: 80%; height: auto;">
</div>

<h3>Steps</h3>
<ol>
    <li>
        <h4>Data Preparation</h4>
        <ul>
            <li>Removed unnecessary columns.</li>
            <li>Eliminated rows with missing data.</li>
            <li>Encoded 'Geography' and 'Gender' using OneHotEncoder.</li>
            <li>Standardized features with StandardScaler.</li>
        </ul>
    </li>
    <li>
        <h4>Data Modeling</h4>
        <ul>
            <li>Trained a Random Forest classifier to predict customer churn.</li>
            <li>Added predicted churn probabilities to the dataset.</li>
        </ul>
    </li>
    <li>
        <h4>Data Connection</h4>
        <ul>
            <li>Imported the CSV file with predicted churn probabilities into Power BI.</li>
        </ul>
    </li>
    <li>
        <h4>Calculations and Features</h4>
        <ul>
            <li>Used the “Group” feature in Power BI to create groups such as age groups and churn probability groups.</li>
            <li>Utilized DAX functions like <code>Calculate</code>, <code>Divide</code>, and <code>DistinctCount</code> to calculate various measures.</li>
            <li>Incorporated an image as a page navigator.</li>
        </ul>
    </li>
</ol>

<h3>Skills Acquired</h3>
<ul>
    <li>Data cleaning, modeling, and prediction using Python.</li>
    <li>Connecting data using import mode in Power BI.</li>
    <li>Calculating measures using DAX.</li>
    <li>Grouping data effectively.</li>
    <li>Implementing page navigation in reports.</li>
</ul>

<h3>Insights and Findings</h3>
<ul>
    <li><strong>Geography:</strong> France exhibits higher churn rates, indicating a need for service improvements.</li>
    <li><strong>Gender:</strong> Female customers are more likely to churn.</li>
    <li><strong>Credit Score:</strong> Lower credit scores are associated with higher churn, suggesting that support services may help. However, some high-score customers also churn, potentially seeking better services.</li>
    <li><strong>Tenure:</strong> Shorter tenures are linked to higher churn, highlighting the importance of improving the onboarding process.</li>
    <li><strong>Age:</strong> Young adults and middle-aged customers have higher churn rates, necessitating targeted products.</li>
    <li><strong>Salary:</strong> Middle-income customers, along with some high-income customers, churn more frequently, possibly due to perceptions of service value.</li>
</ul>

<h3>Recommendations</h3>
<ul>
    <li><strong>Geographical Focus:</strong> Investigate the reasons behind high churn in France and enhance services accordingly.</li>
    <li><strong>Gender-specific Strategies:</strong> Develop retention efforts tailored to female customers.</li>
    <li><strong>Credit Score Segmentation:</strong> Provide support for low-score customers and offer better options for high-score ones.</li>
    <li><strong>Improving Onboarding:</strong> Enhance initial customer experiences to boost retention.</li>
    <li><strong>Tailored Financial Products:</strong> Design financial products specifically for younger and middle-aged customers.</li>
    <li><strong>Competitive Pricing and Services:</strong> Review and improve service value for middle-income customers.</li>
    <li><strong>Credit Card Improvements:</strong> Upgrade credit card offerings to meet customer expectations.</li>
</ul>
<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->
<h1>USECASE 02 - Order Aggregate & Line Analysis</h1>

<h3>Objective</h3>
<p>To analyze and enhance service level performance by examining key metrics such as on-time delivery (OT), in-full delivery (IF), on-time in-full delivery (OTIF), line item fill rate (LIFR), and volume fill rate (VOFR) across different product categories, cities, and customer names. The goal is to identify areas for improvement and implement strategies to boost service efficiency and customer satisfaction.</p>

<h3>Report View</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/20d33d99-2bec-4faf-ab8b-f664a75bc6d0" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/5fabaf3e-0481-4c51-aec3-4b3bffeb3b18" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/11831550-de51-45e9-9511-1a7411218e3c" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/87e6d295-6498-4c0b-9375-bfe91436d2e3" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/6c927ed5-610e-4c03-8230-60b46a303420" style="width: 80%; height: auto;">
</div>

<h3>Steps</h3>

<ol>
    <li>
        <h4>Data Connection</h4>
        <ul>
            <li>The CSV files were imported into Power BI using Import Mode.</li>
        </ul>
    </li>
    <li>
        <h4>Data Preparation</h4>
        <ul>
            <li>Adjusted the headers.</li>
            <li>Removed duplicate data.</li>
            <li>Corrected data types for columns.</li>
            <li>Eliminated unnecessary columns.</li>
            <li>Removed rows with missing data.</li>
        </ul>
    </li>
    <li>
        <h4>Data Modelling</h4>
        <ul>
            <li>Connected the tables using a Star Schema with one fact table and five dimension tables.</li>
            <li>Established one-to-many, uni-directional relationships from dimension to fact tables.</li>
        </ul>
    </li>
    <li>
        <h4>Calculations/Features</h4>
        <ul>
            <li>Displayed up and down arrows with conditional formatting based on differences between actual and target metrics.</li>
            <li>Applied conditional formatting to create gradient colors in visuals and generate heatmaps.</li>
            <li>Implemented page navigation buttons for better user interaction.</li>
            <li>Used the Parameter feature to create a slicer for switching between axis values.</li>
            <li>Added sparklines to provide more insights into the metrics.</li>
            <li>Forecasted future sales trends based on historical data.</li>
            <li>Utilized DAX functions such as <code>Average</code>, <code>Calculate</code>, <code>CountRows</code>, and <code>TreatAs</code>.</li>
        </ul>
    </li>
</ol>

<h3>Skills Acquired</h3>
<ul>
    <li>Conditional formatting.</li>
    <li>Using multi-card visuals to compare metrics.</li>
    <li>Calculating measures using DAX.</li>
    <li>Implementing the Parameter feature.</li>
    <li>Creating page navigation buttons.</li>
    <li>Developing heatmaps.</li>
    <li>Forecasting using Line Chart.</li>
</ul>

<h3>Insights</h3>
<ul>
    <li><strong>Geography:</strong> Surat shows the highest on-time percentage (61.21%) and OTIF percentage (30.07%), indicating relatively better performance. Ahmedabad and Vadodara require improvements in OT and OTIF percentages.</li>
    <li><strong>Product Category:</strong> The Dairy and Food categories have higher order quantities and delivered quantities but show significant room for improvement in on-time and in-full deliveries. Beverages perform relatively better in terms of VOFR% (96.59%) and LIFR% (65.96%).</li>
    <li><strong>Customer Analysis:</strong> Customers like Elite Mart, Expert Mart, and Logic Stores show higher on-time and in-full delivery percentages. Atlas Stores and Chiptec Stores have lower OT and IF percentages, indicating a need for targeted service improvement.</li>
</ul>

<h3>Recommendations</h3>
<ul>
    <li><strong>Geographical Focus:</strong> Improve services in Ahmedabad and Vadodara by leveraging insights from Surat.</li>
    <li><strong>Product Category Enhancement:</strong> Optimize logistics for the Dairy and Food categories.</li>
    <li><strong>Customer-specific Strategies:</strong> Target service improvements for Atlas Stores and Chiptec Stores.</li>
    <li><strong>Utilize Learnings:</strong> Regularly employ sparklines, conditional formatting, and heatmaps for ongoing monitoring.</li>
    <li><strong>Leverage Parameters:</strong> Continuously adjust strategies based on dynamic data insights.</li>
</ul>

<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->

<h1>USECASE 03 - Finance Analysis</h1>

<h3>Objective</h3>
<p>To analyze the financial performance of the company from 2018 to 2020, focusing on key metrics such as sales revenue, gross profit, operational profit, PBIT (Profit Before Interest and Taxes), net profit, and EBITDA (Earnings Before Interest, Taxes, Depreciation, and Amortization). The goal is to identify trends, insights, and areas for improvement across all markets.</p>

<h3>Report View </h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/f0e647e6-cb1b-4e0f-83bb-7bdfa49e6441" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/8038f63f-f7ff-4e83-a2f5-69bb82896751" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/23c89ecd-4654-4298-877c-adabbcd54e45" style="width: 80%; height: auto";>
</div>

<h3>Steps</h3>
<ol>
    <li>
        <h4>Data Connection</h4>
        <ul>
            <li>Tables are connected via DirectQuery from an SQL Server database.</li>
        </ul>
    </li>
    <li>
        <h4>Data Modelling</h4>
        <ul>
            <li>Connected tables using a snowflake schema, with dimension tables linking to other dimension tables.</li>
            <li>Established one-to-many, uni-directional relationships from dimension to fact tables.</li>
        </ul>
    </li>
    <li>
        <h4>Data Preparation</h4>
        <ul>
            <li>Adjusted headers.</li>
            <li>Removed duplicate data.</li>
            <li>Corrected column data types.</li>
            <li>Eliminated unnecessary columns.</li>
            <li>Removed rows with missing data.</li>
        </ul>
    </li>
    <li>
        <h4>Calculations/Features</h4>
        <ul>
            <li>Performed time-based calculations without using time intelligence functions.</li>
            <li>Displayed up and down arrows with conditional formatting based on year-over-year performance.</li>
            <li>Applied conditional formatting to show green or red colors in arrows based on year-over-year differences.</li>
            <li>Implemented page navigation buttons for enhanced user interaction.</li>
            <li>Used the Parameter feature to create slicers for switching between axis values.</li>
            <li>Utilized DAX functions such as <code>Average</code>, <code>Calculate</code>, <code>Date</code>, <code>Month</code>, <code>Day</code>, and <code>Format</code>.</li>
            <li>Implemented Row-Level Security (RLS) to provide users with access to data specific to their country.</li>
        </ul>
    </li>
</ol>

<h3>Skills Acquired</h3>
<ul>
    <li>Calculating time based measures without using time intelligence functions.</li>
    <li>Calculating running/cumulative sum.</li>
    <li>Conditional formatting.</li>
    <li>Using multi-card visuals to compare metrics.</li>
    <li>Using kpi visual.</li>
    <li>Calculating measures using DAX.</li>
    <li>Implementing the Parameter feature.</li>
    <li>Creating page navigation buttons.</li>
    <li>Configuring Row-Level Security (RLS) for data access control.</li>
</ul>

<h3>Insights</h3>
<ul>
    <li><strong>Gross Profit:</strong> Surpassed the target by 34.59%, reaching €5.34M against a goal of €3.97M, indicating strong sales performance and effective cost management.</li>
    <li><strong>Operational Profit:</strong> Slightly exceeded the target by 3.15%, achieving €1.52M against a goal of €1.48M, highlighting operational efficiencies with room for improvement.</li>
    <li><strong>PBIT:</strong> Exceeded the target by 4.7%, reaching €1.59M against a goal of €1.52M, reflecting good management of operating expenses.</li>
    <li><strong>Net Profit:</strong> Slightly below the target by 1.01%, reaching €1.29M against a goal of €1.30M, indicating overall effective financial management after accounting for all expenses.</li>
    <li><strong>EBITDA:</strong> Exceeded the target by 11.42%, achieving €2.24M against a goal of €2.01M, demonstrating strong earnings before interest, taxes, depreciation, and amortization.</li>
    <li><strong>Sales Trends:</strong> Total sales to date amounted to €171,086,642, showcasing robust sales performance contributing significantly to gross profit.</li>
    <li><strong>Country-specific Performance:</strong> Financial losses were noted in Australia despite increasing sales revenue from 2018 to 2020. Operational and net profit goals were not met, highlighting specific issues that require attention to improve profitability in the region.</li>
</ul>

<h3>Recommendations</h3>
<ul>
    <li><strong>Enhance Operational Efficiency:</strong> Continue improving processes to boost operational profit and achieve net profit targets.</li>
    <li><strong>Focus on Cost Management:</strong> Maintain strong cost control measures to ensure gross profit remains above targets.</li>
    <li><strong>Monitor Trends:</strong> Regularly review monthly and yearly financial trends to quickly identify and address issues.</li>
    <li><strong>Country-specific Strategies:</strong> Develop tailored strategies for each country, particularly to address financial losses in Australia.</li>
    <li><strong>Increase Sales Initiatives:</strong> Implement targeted sales strategies to further enhance total sales and profitability.</li>
</ul>

<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->

<h1>USECASE 04 - Credit Card Analysis</h1>

<h3>Objective</h3>
<p>To evaluate the credit card usage patterns, loan distribution, customer demographics, customer feedback, and financial performance across various regions and customer segments. The goal is to identify key trends, opportunities for revenue enhancement, areas with potential risks, and strategies to optimize customer engagement, satisfaction, and profitability.</p>

<h3>Report view</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/733ff992-7176-46f1-b4fa-84edc1e2a334" style="width: 80%; height: auto; margin-bottom: 20px;">
   <img src="https://github.com/user-attachments/assets/a81272c4-b29b-4b6a-8de6-d002061a96a9" style="width: 80%; height: auto; margin-bottom: 20px;">
   <img src="https://github.com/user-attachments/assets/86d8cbb7-d4c2-4723-93f9-e4fea046a4ae" style="width: 80%; height: auto; margin-bottom: 20px;">
   <img src="https://github.com/user-attachments/assets/468e834d-bed0-43a0-98e8-8d92eeb79926" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/33f601a0-6aa0-4fb2-ad09-871f70c8e799" style="width: 80%; height: auto;">
</div>

<h3>Steps</h3>
<ol>
    <li><strong>Data Connection</strong>
        <ul>
            <li>Tables are connected via DirectQuery from an SQL Server database.</li>
        </ul>
    </li>
    <li><strong>Data Modelling</strong>
        <ul>
            <li>Connected tables using a snowflake schema, with dimension tables linking to other dimension tables.</li>
            <li>Established one-to-many, uni-directional relationships from dimension to fact tables.</li>
        </ul>
    </li>
    <li><strong>Data Preparation</strong>
        <ul>
            <li>Adjusted headers and corrected column data types.</li>
            <li>Removed duplicate data and unnecessary columns.</li>
            <li>Eliminated rows with missing data.</li>
        </ul>
    </li>
    <li><strong>Calculations/Features</strong>
        <ul>
            <li>Performed time-based calculations without using time intelligence functions.</li>
            <li>Calculated same-period-last-year data without relying on time intelligence.</li>
            <li>Displayed up and down arrows with conditional formatting based on year-over-year performance.</li>
            <li>Applied conditional formatting to highlight performance differences with green or red colors.</li>
            <li>Implemented the Parameter feature to create slicers for switching between axis values.</li>
            <li>Utilized various DAX functions such as <code>Average</code>, <code>Calculate</code>, <code>Date</code>, <code>Month</code>, <code>Day</code>, <code>Format</code>, <code>CountRows</code>, <code>Filter</code>, etc.</li>
        </ul>
    </li>
</ol>

<h3>Skills Acquired</h3>
<ul>
    <li>Calculating time-based measures without using time intelligence functions.</li>
    <li>Implementing running/cumulative sum calculations.</li>
    <li>Applying conditional formatting in visuals.</li>
    <li>Comparing metrics using multi-card visuals.</li>
    <li>Calculating measures using DAX.</li>
    <li>Implementing the Parameter feature for dynamic visualizations.</li>
</ul>

<h3>Insights</h3>
<ol>
    <li><strong>Customer Demographics</strong>
        <ul>
            <li>Female customers dominate the customer base (57.14%), with male customers slightly less at 42.7%.</li>
            <li>The majority of customers fall into the "29-40 years" age group (25.75%), followed by the "41-52 years" group (20.25%).</li>
            <li>Most customers have an annual income greater than 15 LPA (28.26%), indicating a relatively affluent customer base.</li>
        </ul>
    </li>
    <li><strong>Geographical Distribution</strong>
        <ul>
            <li>Uttar Pradesh (20.88%) and Karnataka (20.09%) have the highest concentration of customers.</li>
            <li>Haryana and Goa have the highest percentage of customers with loans disbursed, particularly home loans (59.06%) and car loans (38.59%).</li>
        </ul>
    </li>
    <li><strong>Loan Distribution</strong>
        <ul>
            <li>Home loans are the most popular type of loan (59.06%), followed by car loans (38.59%) and personal loans (33.65%).</li>
            <li>A significant portion of customers have multiple loans, such as home and car loans.</li>
        </ul>
    </li>
    <li><strong>Credit Card Usage</strong>
        <ul>
            <li>There were 6,248 transactions, with an average spend per card of ₹58.79K.</li>
            <li>The groceries category has the highest transaction amount, followed by shopping.</li>
            <li>A total of 86.01M reward points were accumulated, with an average of 505.82 points per card.</li>
        </ul>
    </li>
    <li><strong>Customer Feedback</strong>
        <ul>
            <li>A total of 1,692 feedback entries were recorded, with an average rating of 3.5 out of 5.</li>
            <li>The majority of feedback is related to complaints (59.16%), followed by suggestions (25.65%) and praise (15.19%).</li>
            <li>The highest percentage of ratings fall in the 4-star category (31.50%), indicating mixed customer satisfaction.</li>
        </ul>
    </li>
    <li><strong>Financial Performance</strong>
        <ul>
            <li>Revenue has decreased slightly compared to the previous year by ₹4.50M, and merchant fees saw a reduction of ₹2.52M.</li>
            <li>Interest income is down by ₹1.17M, while penalties have seen a slight increase of ₹0.36M.</li>
            <li>The defaulter rate has marginally increased from 49.24% to 49.36%, indicating potential risk.</li>
        </ul>
    </li>
</ol>

<h3>Recommendations</h3>
<ol>
    <li><strong>Targeted Marketing</strong>
        <ul>
            <li>Focus marketing campaigns on the "29-40 years" and "41-52 years" age groups, as they represent the largest segments.</li>
            <li>Tailor financial products and offers to the high-income group (>15 LPA) to maximize engagement and revenue.</li>
        </ul>
    </li>
    <li><strong>Regional Strategy</strong>
        <ul>
            <li>Enhance financial services and customer support in Uttar Pradesh and Karnataka, given their large customer base.</li>
            <li>Consider region-specific promotions in Delhi and Maharashtra to boost customer engagement.</li>
        </ul>
    </li>
    <li><strong>Product Optimization</strong>
        <ul>
            <li>Given the high popularity of home and car loans, introduce bundled offers or loyalty programs to encourage repeat loans or cross-selling.</li>
            <li>Develop specific credit card reward programs aligned with top merchant categories (e.g., groceries, shopping) to increase card usage.</li>
        </ul>
    </li>
    <li><strong>Customer Feedback Management</strong>
        <ul>
            <li>Prioritize addressing complaints, as they constitute the majority of feedback (59.16%). Improving the complaint resolution process could enhance overall customer satisfaction.</li>
            <li>Encourage customers to provide positive feedback and ratings, possibly through incentives, to boost the overall average rating.</li>
        </ul>
    </li>
    <li><strong>Risk Mitigation</strong>
        <ul>
            <li>Investigate the rising defaulter rates and implement stricter credit monitoring and customer support for at-risk customers.</li>
            <li>Analyze the causes of the revenue decline, particularly in merchant fees and interest income, and consider revising fee structures or introducing new revenue streams.</li>
        </ul>
    </li>
    <li><strong>Customer Engagement</strong>
        <ul>
            <li>Increase customer interaction and feedback collection to improve the average rating, especially focusing on complaint resolution.</li>
            <li>Utilize the insights from reward points distribution to incentivize higher card usage and customer loyalty.</li>
        </ul>
    </li>
</ol>
<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->
<h1>USECASE 05 - Indian Cricket Captains and Players Analysis</h1>

<h3>Objective</h3>
<p>To meticulously evaluate the performances of Indian cricket captains and players in Test and ODI formats, focusing on their contributions to the team's success over different periods. The analysis aims to identify patterns, strengths, and areas of improvement to inform future strategies.</p>

<h3>Report view</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/46682824-beae-43e6-a819-70db7f4bd2a7" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/64703ac7-db0c-4701-8582-f5d37ac17a57" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/f947f2d5-7b21-432b-87b8-22bb6bf81410" style="width: 80%; height: auto;">
</div>

<h3>Steps</h3>
<ol>
    <li><strong>Data Connection</strong>
        <ul>
            <li>Tables are connected via Import mode from a csv file.</li>
        </ul>
    </li>
    <li><strong>Data Modelling</strong>
        <ul>
            <li>Connected tables using a snowflake schema, with dimension tables linking to other dimension tables.</li>
        </ul>
    </li>
    <li><strong>Data Preparation</strong>
        <ul>
            <li>Removed duplicate data and unnecessary columns.</li>
            <li>Eliminated rows with missing data.</li>
            <li>Reviewed historical match data and cleaned it by removing duplicates and handling missing values.</li>
            <li>Constructed a normalized table for captains to reduce cardinality and facilitate detailed analysis in Power BI.</li>
            <li>Standardized player names across all datasets to ensure consistency.</li>
        </ul>
    </li>
    <li><strong>Calculations/Features</strong>
        <ul>
            <li>Applied conditional formatting to gradient colors in visuals</li>
            <li>Used Filters to filter Top N data.</li>
        </ul>
    </li>
</ol>

<h3>Skills Acquired</h3>
<ul>
    <li>Using filters</li>
    <li>Applying conditional formatting in visuals.</li>
    <li>Calculating measures using DAX.</li>
</ul>

<h3>Insights</h3>
<ul>
  <li><strong>Captains' Performance Analysis:</strong></li>
  <ul>
    <li><strong>Kapil Dev's Captaincy:</strong> Led India in 131 Test matches (1982-1986) and 225 ODIs (1982-1992). Achieved a 30.53% win rate in Tests and 52.45% in ODIs, showcasing a higher success rate in the shorter format. Kapil’s leadership coincided with the emergence of a more aggressive and balanced Indian team, especially in ODIs where his all-round skills were pivotal.</li>
    <li><strong>MS Dhoni's Impact:</strong> Played 347 ODIs and transformed the Indian team into a world-class unit, particularly noted for his calm leadership under pressure, leading to notable victories such as the 2007 T20 World Cup and 2011 ODI World Cup.</li>
    <li><strong>Sourav Ganguly's Legacy:</strong> With 334 ODI matches, Ganguly was instrumental in rebuilding the Indian team post the match-fixing scandal, fostering a culture of aggression and self-belief that laid the groundwork for future successes.</li>
  </ul>
  <li><strong>Top Performers in Test Cricket:</strong></li>
  <ul>
    <li><strong>Sachin Tendulkar's Consistency:</strong> Played 200 Test matches, amassing 15,921 runs with an average of 53.78, solidifying his position as one of the greatest batsmen in cricket history. His ability to perform across all conditions and against all opponents made him the backbone of India’s batting for two decades.</li>
    <li><strong>Anil Kumble's Dominance with the Ball:</strong> With 619 wickets in 132 matches, Kumble was the most successful Indian bowler in Tests, known for his relentless accuracy and ability to extract bounce even on flat pitches.</li>
    <li><strong>Emerging Patterns of Success:</strong> The 2000s saw a surge in debutants who later became key players, indicating a successful phase of talent identification and development.</li>
  </ul>
  <li><strong>Top Performers in ODI Cricket:</strong></li>
  <ul>
    <li><strong>Sachin Tendulkar's Unparalleled Legacy:</strong> Accumulated 18,426 runs in 463 ODIs, with a batting average of 44.83, setting numerous records including the first double century in ODI cricket. Tendulkar’s adaptability and longevity set a benchmark for modern cricketers.</li>
    <li><strong>Virat Kohli's Modern Mastery:</strong> With 12,169 runs in ODIs at an average of 59.07, Kohli exemplifies consistency and has been a pivotal figure in India’s batting lineup, particularly in run chases.</li>
    <li><strong>All-Round Contributions:</strong> Players like Kapil Dev and Ravindra Jadeja have excelled as all-rounders, contributing significantly with both bat and ball. Their versatility has often given India a crucial edge in matches.</li>
  </ul>
  <li><strong>Patterns in Player Development:</strong></li>
  <ul>
    <li><strong>Increased Specialization in Roles:</strong> Recent trends indicate a focus on specialization, with bowlers like Jasprit Bumrah and batsmen like Rohit Sharma emerging as key players in their respective domains.</li>
    <li><strong>Shift Towards Fitness and Athleticism:</strong> Modern players like Virat Kohli and Ravindra Jadeja exemplify the shift towards higher fitness standards, leading to improved fielding and overall team agility.</li>
  </ul>
</ul>

<h3>Recommendations</h3>
<ul>
  <li>Develop Future Leaders: Implement leadership programs based on the strengths of captains like MS Dhoni and Sourav Ganguly, focusing on mental toughness and team unity.</li>
  <li>Cultivate All-Rounders: Prioritize the development of versatile players who can contribute with both bat and ball, inspired by legends like Kapil Dev and Ravindra Jadeja.</li>
  <li>Use Data Analytics: Leverage advanced analytics to identify and nurture emerging talent, focusing on early signs of excellence in domestic and international cricket.</li>
  <li>Prioritize Fitness: Invest in fitness and conditioning programs to maintain high performance levels, taking cues from the fitness regimes of players like Virat Kohli.</li>
  <li>Promote Consistency: Encourage players to develop consistent performances across formats, inspired by the careers of Sachin Tendulkar and Rahul Dravid.</li>
</ul>

<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->

<h1>USECASE 06 - Store Sales Analysis Dashboard</h1>
 
<h3>Objective</h3>
This dashboard aims to provide a comprehensive analysis of store sales performance across different countries, product categories, and time periods. It focuses on identifying key trends, high-performing products, and areas for improvement to optimize sales strategies and enhance overall business performance.

<h3>Report view</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/34c3ad19-c9c8-49b8-8bd9-d1b2010d7e41" style="width: 80%; height: auto; margin-bottom: 20px;">
</div>

<h3>Steps</h3>
<ol>
    <li><strong>Data Connection</strong>
        <ul>
            <li>Imported tables from a CSV file using Import mode.</li>
        </ul>
    </li>
    <li><strong>Data Modelling</strong>
        <ul>
            <li>Connected tables using a Star Schema with one fact table and multiple dimension tables.</li>
            <li>Established one-to-many, unidirectional relationships from dimension tables to the fact table.</li>
        </ul>
    </li>
    <li><strong>Data Preparation</strong>
        <ul>
            <li>Removed duplicate entries and unnecessary columns.</li>
            <li>Eliminated rows with missing data to ensure accuracy.</li>
        </ul>
    </li>
    <li><strong>Calculations/Features</strong>
        <ul>
            <li>Applied conditional formatting to gradient colors in a gauge visual, highlighting the red and green sections of the axis.</li>
            <li>Calculated total sales over time using time intelligence functions.</li>
            <li>Dynamically displayed the Top N products using a slicer and rank function.</li>
            <li>Calculated running totals.</li>
            <li>Utilized a calendar dimension table for time-based calculations.</li>
            <li>Employed DAX functions such as <code>SUM</code>, <code>RANK</code>, <code>SAMEPERIODLASTYEAR</code>, <code>EXCEPT</code>, and <code>CALCULATE</code>.</li>
        </ul>
    </li>
</ol>

<h3>Skills Acquired</h3>
<ul>
    <li>Effectively using filters to refine data.</li>
    <li>Applying conditional formatting in visuals to enhance readability.</li>
    <li>Calculating measures using DAX for advanced data analysis.</li>
</ul>

<h3>Insights</h3>
<ul>
    <li>Geography: France and the UK show significant sales figures, but France underperforms in goal achievement, indicating potential for improvement in sales strategies.</li>
    <li>Product Categories: Electronics dominate the sales, with TVs and Gaming Laptops being the top sellers, suggesting a strong consumer preference for these items.</li>
    <li>Time Period: Sales data reveals a peak in Q3 2020 and a notable decline in early 2024, indicating seasonal trends and possibly the impact of external factors on sales.</li>
    <li>Sales Performance: Highest sales were recorded on 13-09-2020 with $11,078.14, highlighting the impact of specific events or promotions on sales.</li>
    <li>Top Products: Top-selling products include TVs, Gaming Laptops, and Washing Machines, showing a preference for high-value electronics and essential appliances.</li>
    <li>Overall Performance: Despite achieving a lifetime sales total of $1,512,172.14, the goal achievement of -12.39% suggests room for improvement in reaching sales targets.</li>
</ul>

<h3>Recommendations</h3>
<ul>
    <li>Enhance sales strategies in France to meet targets.</li>
    <li>Offer promotions for popular electronics.</li>
    <li>Replicate successful Q3 2020 strategies.</li>
    <li>Run targeted campaigns during low sales periods.</li>
    <li>Focus on high-value products to boost revenue.</li>
    <li>Adjust sales targets to align with market trends.</li>
</ul>
    <hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->
<h1>USECA 07 - IPL Performance Analysis</h1>

<h3>Objective:</h3>
To analyze IPL matches, performance metrics, player statistics, venue statistics and historical data to identify key trends, top performers, and strategic insights for improving team performance

<h3>Dashboard:</h3> 
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/e9993bd7-0c39-4cc2-99f1-510c36c4bfe9" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/748438dc-d1b4-4470-8185-8fcaca2c5cc8" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/94d50fb6-f611-42d0-9493-8c5efe77da07" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/efb8ff77-d86b-41c9-bdba-5511656fad0e" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/688653e6-bae7-43d3-a896-ea315b333601" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/234e556a-f845-493c-bd7d-53fe7ee7ab8b" style="width: 80%; height: auto;">
</div>

<h3>Data Preparation:</h3>
<ul>
  <li>Removed Unnecessary Columns: Identified and removed columns not essential for the analysis</li>
  <li>Handled Missing Data: Dropped rows with missing values to ensure data integrity</li>
  <li>Removed Duplicates: Eliminated duplicate entries to maintain accurate results</li>
  <li>Features Used:
    <ul>
      <li>Added buttons for easy page navigation</li>
      <li>Dax calculations functions: Caculate, Summarise, Filter, Divide, Concat to calculate various measure like economy rate, average, strike rate, etc</li>
    </ul>
  </li>
</ul>

<h3>Data Modelling:</h3>
<ul>
  <li>Tables were connected using one-to-many relationships based on Match ID</li>
</ul>

<h3>Key Explorations:</h3>
<ul>
  <li>Match Outcomes: Analyzed the number of wins in chasing versus defending across different venues and explored the total number of matches and their outcomes</li>
  <li>Runs and Wickets: Investigated total runs scored by season, total wickets taken, and boundaries hit Analyzed runs scored by different overs and innings</li>
  <li>Venue Analysis: Examined performance metrics such as wins, economy rates, and matches hosted by various venues</li>
  <li>Player Performance: Reviewed leading wicket-takers, total runs scored, boundaries conceded, and extras by bowlers Analyzed runs in single overs and stumpings by players</li>
</ul>

<h3>Insights:</h3>
<ul>
  <li>Match Outcomes: More wins in chasing (554) compared to wins in defending (459) Teams might prefer chasing, indicating a strategic trend</li>
  <li>Runs and Wickets: Total runs scored have fluctuated over the years, with peaks in certain years Trends can indicate changing strategies or player form</li>
  <li>Venue Performance:
    <ul>
      <li>Best Venue for Bowlers: OUTsurance Oval has the lowest economy rate, favoring bowlers</li>
      <li>Best Venue for Batting: Barsapra Cricket Stadium has the highest economy rate, favoring batsmen</li>
    </ul>
  </li>
  <li>Player Performance: Players like Virat Kohli and AB de Villiers lead in total runs, while bowlers like YS Chahal and DJ Bravo lead in wickets Key players' performance is crucial to team success</li>
  <li>Team Performance: Teams like MI (Mumbai Indians) and CSK (Chennai Super Kings) show strong performance in both defending and chasing Consistent strategies and strong player rosters contribute to their success</li>
</ul>
<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->
<h1>Bank Loan Analysis</h1>

<h3>Objective:</h3> To analyze customer demographics and loan data to identify trends and provide actionable insights for improving loan products and marketing strategies.

<h3>Dashboard:</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/ash15h/Power-Bi-Dashboards/assets/67120563/b00d2564-e22c-4d01-9ea9-ea0e2f8a71de" style="width: 80%; height: auto;">
</div>

<h3>Data Preparation:</h3>
<ul>
<li>Removed Unnecessary Columns: Kept only columns relevant to the analysis</li>
<li>Handled Missing Data: Dropped rows with missing values</li>
<li>Removed Duplicates: Eliminated duplicate entries</li>
</ul>

<h3>Key Explorations:</h3>
  <ul>
    <li>Customer Demographics: Distribution of housing and other loans by age, job, and marital status</li>
    <li>Loan Data: Monthly disbursement of housing and other loans, job-wise loan distribution, and loans by age and marital status</li>
  </ul>
</li>
</ul>

<h3>Insights:</h3>
<ul>
<li>Age Groups:
  <ul>
    <li>Observation: 31-40 age group has the most housing loans; 19-30 age group prefers other loans</li>
    <li>Implication: Target marketing for younger customers with specific loan products</li>
  </ul>
</li>
<li>Job Categories:
  <ul>
    <li>Observation: Blue-collar and self-employed have the most housing loans; students and unemployed have the least</li>
    <li>Implication: Customize loans for blue-collar and self-employed individuals</li>
  </ul>
</li>
<li>Marital Status:
  <ul>
    <li>Observation: Married individuals take the most loans</li>
    <li>Implication: Develop family-focused loan products</li>
  </ul>
</li>
<li>Monthly Distribution:
  <ul>
    <li>Observation: May has the highest, December the lowest loan disbursements</li>
    <li>Implication: Plan strategic marketing for peak months</li>
  </ul>
</li>
</ul>

<h3>Recommendations:</h3>
<ul>
<li>Target Younger Demographics: Create loans for 19-30 age group inclined towards other loans</li>
<li>Customize for Blue-collar and Self-employed: Offer loan products tailored to their needs</li>
<li>Family-focused Loan Products: Introduce and market family-oriented loans</li>
<li>Seasonal Loan Campaigns: Plan marketing campaigns during peak loan months (e.g., May)</li>
<li>Support for High-risk Jobs: Provide financial advice for customers in high-risk jobs to help manage loans better</li>
</ul>
<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->
<h1>Electoral Bonds Analysis</h1>

<h3>Objective:</h3> 
To analyse the data related to electoral bonds in India, focusing on the total denominations, political parties, purchasers, and trends over the years.

<h3>Dashboard:</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/ash15h/Power-Bi-Dashboards/assets/67120563/0fd9a1fb-141f-4e6e-ad92-0debafacc8de" style="width: 80%; height: auto;">
</div>

<h3>Data Preparation:</h3>
<ul>
  <li>Data Cleaning: Ensure all data entries are correctly formatted, and there are no missing values</li>
  <li>Categorization: Group data by political parties and purchasers to facilitate comparison</li>
  <li>Time Series Analysis: Organize data chronologically to identify trends over the years and quarters</li>
</ul>

<h3>Insights:</h3>
<ul>
  <li>Total Denominations: The total amount of electoral bonds purchased is ₹121.56 billion</li>
  <li>Political Parties: 24 political parties have received electoral bonds. The Bharatiya Janata Party (BJP) received almost half of the total denominations, while the denomination received by All India Congress Committee is significantly lower</li>
  <li>Purchasers: 1320 purchasers have bought electoral bonds, with Future Gaming and Hotel Services PR making the highest denominations</li>
  <li>Yearly Trends: The total denominations increased significantly in certain years, with notable spikes in 2020 and 2022</li>
  <li>Quarterly Trends: Quarter 2 and Quarter 4 show higher denominations compared to Quarter 1 and Quarter 3</li>
</ul>

<h3>Recommendations:</h3>
<ul>
  <li>Public Awareness: Increase public awareness about electoral bonds and their impact on political funding and elections</li>
</ul>
<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->
