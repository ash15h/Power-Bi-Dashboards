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

<h1>USECASE 04 - Paris Olympics Analysis</h1>

<h3>Objective:</h3> 
To analyze and provide key insights on the Paris Olympics, focusing on aspects such as participating countries, events, athletes, historical performance, and key achievements.

<h3>Report View:</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/4596b418-4e79-4d71-b00d-827188a31292" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/292757e3-df82-4851-9078-f9c7d505a894" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/dd56d3c4-6a68-4b3f-bea3-20927e646e0b" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/63e1c48d-f843-4be4-8352-2ade161359f2" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/7aacd41f-7e5a-45df-8552-5b1f2becd944" style="width: 80%; height: auto;">
</div>

<h3>Steps</h3>
<ol>
    <li><strong>Data Connection</strong>
        <ul>
            <li>Tables are connected via Import mode using an Excel file.</li>
        </ul>
    </li>
    <li><strong>Data Modeling</strong>
        <ul>
            <li>Tables are connected using a snowflake schema, with dimension tables linked to other dimension tables.</li>
        </ul>
    </li>
    <li><strong>Data Preparation</strong>
        <ul>
            <li>Gathered data on athletes, events, and medals from multiple sources to ensure accuracy.</li>
            <li>Adjusted headers and corrected column data types.</li>
            <li>Removed duplicate data and unnecessary columns.</li>
            <li>Cleaned data to standardize country names, athlete details, and event categories.</li>
        </ul>
    </li>
    <li><strong>Calculations/Features</strong>
        <ul>
            <li>Grouped data by age groups, event categories, and medal types using Power BI’s "Group" feature.</li>
            <li>Utilized various DAX functions such as <code>Calculate</code>, <code>Date</code>, <code>Format</code>, <code>DistinctCount</code>,etc.</li>
        </ul>
    </li>
</ol>

<h3>Skills Acquired</h3>
<ul>
    <li>Calculating measures using DAX.</li>
    <li>Leveraged bookmarks to open and close the side drawer, ensuring data persistence while navigating using bookmarks.</li>
    <li>Implemented page navigation using buttons to enhance user experience.</li>
    <li>Syncing slicers across pages.</li>
</ul>  

<h3>Insights:</h3>
<ul>
  <li><strong>Participation:</strong> The Paris Olympics have seen increased participation from emerging countries, highlighting a broader global interest in the Games.</li>
  <li><strong>Top-performing Nations:</strong> Certain countries continue to dominate in specific sports, showcasing long-standing strengths in areas like athletics and swimming.</li>
  <li><strong>Purchasers:</strong> 1320 purchasers have bought electoral bonds, with Future Gaming and Hotel Services PR making the highest denominations</li>
  <li><strong>Gender Representation:</strong> There is a balanced representation of male and female athletes, indicating significant strides in gender inclusivity over recent years.</li>
  <li><strong>Youth Athletes:</strong> A substantial presence of young athletes points toward a generational shift in Olympic competitors.</li>
  <li><strong>Popular Sports:</strong> Track and field events have seen the highest participation, emphasizing their global appeal.</li>
</ul>

<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->

<h1>USECASE 05 - Credit Card Analysis</h1>

<h3>Objective</h3>
<p>To evaluate the credit card usage patterns, loan distribution, customer demographics, customer feedback, and financial performance across various regions and customer segments. The goal is to identify key trends, opportunities for revenue enhancement, areas with potential risks, and strategies to optimize customer engagement, satisfaction, and profitability.</p>

<h3>Report view</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/c6248c04-f1ba-48f6-a86f-7566b8c8efa7" style="width: 80%; height: auto; margin-bottom: 20px;">
   <img src="https://github.com/user-attachments/assets/9dd02996-aaf0-4e14-a7a0-ef27c3806c23" style="width: 80%; height: auto; margin-bottom: 20px;">
   <img src="https://github.com/user-attachments/assets/584be58d-d6b1-4316-9c3b-980476c935b4" style="width: 80%; height: auto; margin-bottom: 20px;">
   <img src="https://github.com/user-attachments/assets/eb6a0dee-2f76-4e4f-b6da-f7d8cddc72cd" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/e709db34-a49f-4540-b843-84ebc8fa1c2e" style="width: 80%; height: auto;">
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
            <li>Implemented the Parameter feature to create slicers for switching between axis values.</li>
            <li>Utilized various DAX functions such as <code>Average</code>, <code>Calculate</code>, <code>Date</code>, <code>Month</code>, <code>Day</code>, <code>Format</code>, <code>CountRows</code>, <code>Filter</code>,<code>RankX</code> etc.</li>
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
    <li>Usinf RankX function to calculate Top N performers.</li>
</ul>

<h3>Insights</h3>
<ol>
    <li><strong>Customer Demographics</strong>
        <ul>
            <li>Female customers dominate the customer base, accounting for 58.4%, with male customers at 41.2%.</li>
            <li>The most represented age group is "29-40 years" (25.75%), followed by "41-52 years" (20.25%).</li>
            <li>Customers with an annual income greater than ₹15 LPA form the largest segment (28.26%).</li>
        </ul>
    </li>
    <li><strong>Geographical Distribution</strong>
        <ul>
            <li>Uttar Pradesh (21.68%) and Karnataka (19.44%) have the highest concentrations of customers.</li>
            <li>Haryana and Delhi are notable for high loan disbursements, particularly home loans (42.83%).</li>
        </ul>
    </li>
    <li><strong>Loan Distribution</strong>
        <ul>
            <li>Home loans are the most common (63.75%), followed by car loans (24.06%) and personal loans (22.49%).</li>
            <li>Customers with multiple loans, such as home and car loans, represent a growing segment.</li>
        </ul>
    </li>
    <li><strong>Credit Card Usage</strong>
        <ul>
            <li>Total transactions amounted to ₹2.70 billion, with an average spend of ₹1.09M per card.</li>
            <li>Groceries and shopping are the top categories by transaction amount.</li>
            <li>Platinum and Gold cards are the most preferred, each accounting for around 25% of total card users.</li>
        </ul>
    </li>
    <li><strong>Customer Feedback</strong>
        <ul>
            <li>A total of 4,432 feedback entries were recorded, with an average satisfaction rating of 3.5 out of 5.</li>
            <li>Complaints dominate the feedback (59.57%), followed by suggestions (25%) and praise (15.43%).</li>
            <li>Most ratings fall in the 4-star category (31.23%).</li>
        </ul>
    </li>
    <li><strong>Financial Performance</strong>
        <ul>
            <li>Revenue increased by ₹82.29M compared to the previous year.</li>
            <li>Merchant fees saw a significant rise of ₹49.22M.</li>
            <li>The defaulter rate slightly increased from 49.10% to 49.67%, indicating a potential risk.</li>
        </ul>
    </li>
</ol>

<h3>Recommendations</h3>
<ol>
    <li><strong>Targeted Marketing</strong>
        <ul>
            <li>Focus marketing campaigns on the "29-40 years" age group and customers earning more than ₹15 LPA.</li>
            <li>Tailor credit card offers and loan products to match customer preferences in groceries and shopping.</li>
        </ul>
    </li>
    <li><strong>Regional Strategy</strong>
        <ul>
            <li>Enhance customer services and financial product offerings in Uttar Pradesh and Karnataka to capitalize on their large customer base.</li>
            <li>Conduct targeted campaigns in Haryana and Delhi for promoting home and car loans.</li>
        </ul>
    </li>
    <li><strong>Product Optimization</strong>
        <ul>
            <li>Develop bundled offers for multiple loans (e.g., home and car loans) to encourage cross-selling.</li>
            <li>Introduce loyalty programs for Platinum and Gold card users to boost retention and spending.</li>
        </ul>
    </li>
    <li><strong>Customer Feedback Management</strong>
        <ul>
            <li>Prioritize resolving complaints efficiently to improve the satisfaction rating.</li>
            <li>Encourage more positive feedback through incentives for high ratings and testimonials.</li>
        </ul>
    </li>
    <li><strong>Risk Mitigation</strong>
        <ul>
            <li>Monitor the rising defaulter rate closely and implement preemptive measures for at-risk customers.</li>
            <li>Analyze revenue components to sustain the positive growth trend and explore diversification in merchant fees and interest income.</li>
        </ul>
    </li>
    <li><strong>Customer Engagement</strong>
        <ul>
            <li>Use insights from transaction data to personalize customer offers and reward programs.</li>
            <li>Increase feedback collection frequency and improve the overall rating by focusing on quick resolution of issues.</li>
        </ul>
    </li>
</ol>

<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->
<h1>USECASE 06 - Indian Cricket Captains and Players Analysis</h1>

<h3>Objective</h3>
<p>To meticulously evaluate the performances of Indian cricket captains and players in Test and ODI formats, focusing on their contributions to the team's success over different periods. The analysis aims to identify patterns, strengths, and areas of improvement to inform future strategies.</p>

<h3>Report view</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/dc2fd6ae-bf0b-4fb1-bed5-9189f62f6377" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/2f21c8e5-758a-48c8-bfca-cb76ac8db6b7" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/4afe9635-b89f-4a67-8f49-0f57d022227d" style="width: 80%; height: auto;">
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
            <li>Constructed a normalized table for captains to reduce dimensionality and facilitate detailed analysis in Power BI.</li>
            <li>Standardized player names across all datasets to ensure consistency.</li>
        </ul>
    </li>
    <li><strong>Calculations/Features</strong>
        <ul>
            <li>Applied conditional formatting to gradient colors in visuals</li>
            <li>Used Filters to filter Top N data.</li>
            <li>Implemented page navigation buttons for better user interaction.</li>
        </ul>
    </li>
</ol>

<h3>Skills Acquired</h3>
<ul>
    <li>Using filters</li>
    <li>Applying conditional formatting in visuals.</li>
    <li>Calculating measures using DAX.</li>
    <li>Implementing page navigation buttons.</li>
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

<h1>USECASE 07 - Store Sales Analysis Dashboard</h1>
 
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
<h1>USECASE 08 - IPL Performance Analysis</h1>

<h3>Objective</h3>
<p>The objective of the IPL Dashboard is to provide a comprehensive analysis of team and player performances across various IPL seasons. It focuses on key metrics such as runs, wickets, and match outcomes. The dashboard is designed to help identify patterns, top performers, and areas of improvement for teams and players.</p>

<h3>Report view</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/265a8cce-ffb6-43ce-8a0a-b4b28ec7330c" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/9d68a0f8-2dc5-4d3c-865b-181c6998ad2c" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/093ef66a-6529-49bf-923c-160c31ebee53" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/18dc63a3-fb0d-4c2c-b018-5289ebb832f8" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/eb937a50-f9ab-408b-b20a-91890b8524e2" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/f5878a22-658a-4e17-9cf8-4e8d7432abb6" style="width: 80%; height: auto;">
</div>

<h3>Steps</h3>
<ol>
    <li><strong>Data Connection</strong>
        <ul>
            <li>Tables are connected using Import mode from a CSV file.</li>
        </ul>
    </li>
    <li><strong>Data Modeling</strong>
        <ul>
            <li>Tables are connected using a snowflake schema, with dimension tables linked to other dimension tables.</li>
        </ul>
    </li>
    <li><strong>Data Preparation</strong>
        <ul>
            <li>Removed duplicate data.</li>
            <li>Removed unnecessary columns.</li>
            <li>Eliminated rows with missing data.</li>
            <li>Reviewed historical match data and cleaned it by removing duplicates and handling missing values.</li>
            <li>Constructed a normalized table to reduce cardinality and facilitate detailed analysis in Power BI.</li>
            <li>Replaced inconsistent values in columns across tables.</li>
        </ul>
    </li>
    <li><strong>Calculations/Features</strong>
        <ul>
            <li>Used the “Group” feature in Power BI to create groups for over ranges.</li>
            <li>Filtered data in visuals to obtain the Top N players for the selected category.</li>
            <li>Defined measures for conditionally formatting column's color in visual.</li>
            <li>Implemented page navigation buttons for enhanced user interaction.</li>
            <li>DAX functions like <code>IsBlank</code>, <code>RankX</code>, <code>CountRows</code>, <code>SelectedValue</code>, <code>Switch</code>, and <code>Count</code> were utilized.</li>
        </ul>
    </li>
</ol>

<h3>Skills Acquired</h3>
<ul>
    <li>Connecting data using Import mode in Power BI.</li>
    <li>Applying field value for conditional formatting.</li>
    <li>Calculating measures using DAX.</li>
    <li>Grouping data effectively.</li>
    <li>Implementing page navigation in reports.</li>
</ul>

<h3>Insights</h3>
<ul>
    <li><strong>Top Teams:</strong> CSK, MI, and KKR consistently dominate in terms of playoff appearances and winning percentages, highlighting their strong performance across seasons.</li>
    <li><strong>Batting Performance:</strong> 
        <ul>
            <li>Virat Kohli and Shikhar Dhawan are among the top run-scorers, showcasing their consistency across different seasons.</li>
            <li>MS Dhoni excels in the death overs, establishing himself as one of the most reliable finishers in IPL history.</li>
            <li>Chris Gayle and Rohit Sharma are among the top six-hitters, indicating their aggressive batting styles.</li>
        </ul>
    </li>
    <li><strong>Bowling Performance:</strong> 
        <ul>
            <li>YS Chahal and DJ Bravo are leading wicket-takers, especially in crucial overs, making them essential to their teams' success.</li>
            <li>Bhuvneshwar Kumar and Sandeep Sharma excel in the powerplay, demonstrating their ability to provide early breakthroughs.</li>
        </ul>
    </li>
    <li><strong>Venue Analysis:</strong> 
        <ul>
            <li>M. Chinnaswamy Stadium and Wankhede Stadium are favorable venues for batsmen, with players like Virat Kohli and AB de Villiers scoring heavily here.</li>
            <li>MA Chidambaram Stadium is a fortress for CSK, reflecting their home advantage.</li>
        </ul>
    </li>
    <li><strong>Seasonal Patterns:</strong> 
        <ul>
            <li>Teams like GT and LSG have shown remarkable consistency in their early years, with high winning percentages and strong performances in key matches.</li>
            <li>Recent seasons have seen a rise in the importance of all-rounders, with players like Ravindra Jadeja excelling in both batting and bowling departments.</li>
        </ul>
    </li>
</ul>

<h3>Recommendations</h3>
<ul>
    <li><strong>Focus on Consistency:</strong> Teams should prioritize consistent performers like Virat Kohli and MS Dhoni, who can anchor the innings and provide stability under pressure.</li>
    <li><strong>Strengthen Death Over Strategies:</strong> Investing in bowlers like DJ Bravo and Lasith Malinga, who excel in death overs, could significantly improve match outcomes, especially in tight situations.</li>
    <li><strong>Leverage Home Advantage:</strong> Teams should develop strategies tailored to their home grounds, similar to CSK's dominance at MA Chidambaram Stadium, to maximize their chances of success.</li>
    <li><strong>Develop Young Talent:</strong> Emerging teams like GT and LSG should focus on nurturing young talent to maintain their early momentum and build a strong foundation for the future.</li>
    <li><strong>Adapt to Venue Conditions:</strong> Players and teams should continuously adapt their strategies based on venue-specific data, ensuring optimal performance across different stadiums.</li>
</ul>

<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->
<h1>USECASE 09 - Compliance & Security Dashboard</h1>

<h3>Objective</h3>
<p>To monitor and analyze security & compliance issues across multiple domains, track ownership through SPOCs and testers, and provide visibility into issue status, due dates, and workloads. The goal is to improve operational transparency, prioritize risks, and ensure timely resolution of compliance tasks.</p>

<h3>Report View</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/ae14ade2-23f8-42ff-839b-21da7ddd65de" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/c6ec209c-1f89-4504-ad06-42a7b411dced" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/016d7bb6-2e9b-4d90-9eed-1cb3fbf9c200" style="width: 80%; height: auto;">
</div>

<h3>Steps</h3>
<ol>
  <li>
    <h4>Data Connection</h4>
    <ul>
      <li>Tables are connected using Import mode from a CSV file.</li>
      <li>Implemented a Star Schema for efficient modeling and relationships.</li>
      <li>Created a Bridge Table using DAX to eliminate many-to-many relationships.</li>
    </ul>
  </li>
  <li>
    <h4>Data Preparation</h4>
    <ul>
      <li>Adjusted headers and corrected column data types.</li>
      <li>Removed duplicate records and unnecessary columns.</li>
      <li>Introduced a Bridge Table to enable clean relational mapping.</li>
    </ul>
  </li>
  <li>
    <h4>Calculations and Features</h4>
    <ul>
      <li>Used Drill Through functionality to navigate to detailed Issue Details page.</li>
      <li>Implemented the Parameter feature to dynamically switch axis values.</li>
      <li>Used <code>Summarize</code>, <code>DistinctCount</code> and various DAX functions to compute custom metrics.</li>
    </ul>
  </li>
</ol>

<h3>Skills Acquired</h3>
<ul>
  <li>Designing and modeling data using Star Schema.</li>
  <li>Using Bridge Tables to manage complex relationships.</li>
  <li>Implementing Drill Through and Parameter features in Power BI.</li>
  <li>Advanced use of DAX for summarization and calculation.</li>
</ul>

<h3>Insights and Findings</h3>
<ul>
  <li><strong>SPOC Activity:</strong> Angela, Robin, and Cassey are the most active SPOCs, indicating a potential need for task redistribution.</li>
  <li><strong>Tester Workload:</strong> Fiona and Bob handle the most CT requests — optimization opportunities may exist here.</li>
  <li><strong>Domain-wise Issue Volume:</strong> AuthTrack, CoreOps, and StratOps consistently report more issues, which may indicate higher vulnerability or reporting maturity.</li>
  <li><strong>Overdue Issues:</strong> Multiple tasks are past due, some significantly, pointing to process bottlenecks or follow-up gaps.</li>
</ul>

<h3>Recommendations</h3>
<ul>
  <li><strong>Balance SPOC Responsibilities:</strong> Evaluate and distribute workload more evenly across SPOCs.</li>
  <li><strong>Monitor Tester Capacity:</strong> Track and manage tester workload to ensure efficiency.</li>
  <li><strong>Prioritize High-Issue Domains:</strong> Conduct root-cause analysis for frequently reported domains.</li>
  <li><strong>Follow-up for Overdue Issues:</strong> Set up automated alerts or reminders for past-due items.</li>
  <li><strong>Enhance Drill-through Pages:</strong> Enrich detail views with resolution time, test status, and SLA indicators.</li>
  <li><strong>Track SLAs Visually:</strong> Introduce timeline visuals to monitor adherence to delivery expectations.</li>
</ul>

<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->

<h1>USECASE 10 - Bank Loan Analysis</h1>

<h3>Objective</h3> To analyze customer demographics and loan data to identify trends and provide actionable insights for improving loan products and marketing strategies.

<h3>Report view</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/cea26c03-2708-4287-bfe1-f6e81cdf2359" style="width: 80%; height: auto;">
</div>

<h3>Steps</h3>
<ol>
    <li><strong>Data Connection</strong>
        <ul>
            <li>Tables are connected via Import mode using an Excel file.</li>
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
            <li>Implemented the Parameter feature to create slicers for switching between axis values.</li>
            <li>Utilized various DAX functions such as <code>Average</code>, <code>Calculate</code>, <code>Date</code>, <code>Month</code>, <code>Day</code>, <code>Format</code>, <code>CountRows</code>, <code>Filter</code>, etc.</li>
        </ul>
    </li>
</ol>

<h3>Skills Acquired</h3>
<ul>
    <li>Calculating measures using DAX.</li>
    <li>Implementing the Parameter feature for dynamic visualizations.</li>
</ul>

<h3>Insights</h3>
<ul>
<li>Age Groups:
  <ul>
    <li><strong>Observation:</strong> 31-40 age group has the most housing loans; 19-30 age group prefers other loans</li>
    <li><strong>Implication:</strong> Target marketing for younger customers with specific loan products</li>
  </ul>
</li>
<li>Job Categories:
  <ul>
    <li><strong>Observation:</strong> Blue-collar and self-employed have the most housing loans; students and unemployed have the least</li>
    <li><strong>Implication:</strong> Customize loans for blue-collar and self-employed individuals</li>
  </ul>
</li>
<li>Marital Status:
  <ul>
    <li><strong>Observation:</strong> Married individuals take the most loans</li>
    <li><strong>Implication:</strong> Develop family-focused loan products</li>
  </ul>
</li>
<li>Monthly Distribution:
  <ul>
    <li><strong>Observation:</strong> May has the highest, December the lowest loan disbursements</li>
    <li><strong>Implication:</strong> Plan strategic marketing for peak months</li>
  </ul>
</li>
</ul>

<h3>Recommendations:</h3>
<ul>
<li><strong>Target Younger Demographics:</strong> Create loans for 19-30 age group inclined towards other loans</li>
<li><strong>Customize for Blue-collar and Self-employed:</strong> Offer loan products tailored to their needs</li>
<li><strong>Family-focused Loan Products:</strong> Introduce and market family-oriented loans</li>
<li><strong>Seasonal Loan Campaigns:</strong> Plan marketing campaigns during peak loan months (e.g., May)</li>
<li><strong>Support for High-risk Jobs:</strong> Provide financial advice for customers in high-risk jobs to help manage loans better</li>
</ul>
<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->
<h1>USECASE 11 - Bank Loan Analysis</h1>

<h3>Objective</h3> To analyze retail sales performance by tracking key metrics across regions, products, and time periods, enabling stakeholders to identify trends, assess targets, and make data-driven decisions.

<h3>Report view</h3>

<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/user-attachments/assets/86a252b4-f2f5-4a97-a4f4-0368aaab143b" style="width: 80%; height: auto;">
</div>

<h3>Steps</h3>
<ol>
    <li><strong>Data Connection</strong>
        <ul>
            <li>Source Integration: Historical data files from a local folder were imported and combined to create a unified dataset whereas Dimension table were fetched from PostgreSQL database.</li>
        </ul>
    </li>
    <li><strong>Data Modelling</strong>
        <ul>
            <li>Schema: Organized in a Snowflake schema with a central Fact Sales table linked to dimension tables for date, country, product, and sales representatives.</li>
          <li>Connections: Utilized Import mode for sales data, with real-time updates via DirectQuery for dimension tables in PostgreSQL.</li>
    </li>
    <li><strong>Data Preparation</strong>
        <ul>
           <li>Data Cleaning: Standardized headers, removed duplicates, and formatted data consistently.</li>
          <li>Transformation: Created new columns for date using "Column by Example" for better formatting</li>
      <li>Time Support: Added a date lookup table for time-based calculations.</li>
        </ul>
    </li>
    <li><strong>Calculations/Features</strong>
        <ul>
            <li>DAX Functions: Used CALCULATE, AVERAGE, and SUM for metrics, and time functions like PREVIOUSQUARTER() for period comparisons.</li>
            <li>Date Calculations: Employed CALENDAR() to create a date lookup table for consistency in date-based analysis.</li>
          <li>Icon Indicators: Used icons to display growth or decline in average revenue and profit, giving quick visual cues on daily trends.</li>
        </ul>
    </li>
</ol>

<h3>Skills Acquired</h3>
<ul>
    <li>Advanced DAX functions for KPI calculations and time intelligence.</li>
    <li>Proficiency in data cleaning, Snowflake schema modeling, and applying Import, Dual, and DirectQuery modes.</li>
</ul>

<h3>Insights</h3>
<ul>
<li>Revenue & Units Sold: Declines noted in recent quarters, possibly indicating seasonal or emerging challenges.</li>
<li>Top Performers: Specific products and sales reps, notably "El Bob" and "Jan Novotny," significantly contribute to revenue.</li>
<li>Profit Volatility: Monthly Gross Profit Percent shows fluctuations, suggesting areas for deeper analysis.</li>
</ul>

<h3>Recommendations:</h3>
<ul>
<li>Investigate declining metrics to identify underlying issues.</li>
<li>Apply successful strategies from high-performing products and reps to improve other areas.</li>
<li>Further analyze Gross Profit Percent fluctuations to manage profit stability.</li>
<li>Add filters or drill-downs for more granular analysis by region and product category.</li>
</ul>
<hr style="border: 1px solid #fff; margin: 20px 0;">
