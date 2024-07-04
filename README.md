<h1>Cricket Performance Analysis</h1>

<h3>Objective:</h3>
To analyze Indian cricketers' match statistics, performance metrics, and historical data to identify key trends, top performers, and strategic insights for improving team performance.

<h3>Dashboard:</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/ash15h/Power-Bi-Dashboards/assets/67120563/4dd63760-9339-4fc5-bf22-a93bac3fe3c0" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/ash15h/Power-Bi-Dashboards/assets/67120563/59ee9f60-7b31-4a2d-b98e-c42cca02dfc8" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/ash15h/Power-Bi-Dashboards/assets/67120563/ab5f713d-feb3-4561-a610-3efaea60cc6e" style="width: 80%; height: auto; margin-bottom: 20px;">
</div>

<h3>Data Preparation:</h3>
<ul>
  <li>Removed Unnecessary Columns: Identified and removed columns not essential for the analysis.</li>
  <li>Handled Missing Data: Dropped rows with missing values to ensure data integrity.</li>
  <li>Removed Duplicates: Eliminated duplicate entries to maintain accurate results.</li>
  <li>Feature Engineering: Changed many names to match across all tables.</li>
  <li>Created Captains Table: Created a table with captains' names and images for Power BI's new slicer.</li>
</ul>

<h3>Data Modelling:</h3>
<ul>
  <li>Created a new name lookup table and connected all the tables to it. The relationship was one-to-one.</li>
  <li>Used DAX to calculate various sums, highest scores, and other stats.</li>
</ul>

<h3>Learning:</h3>
The summary page provides an initial overview, with additional pages hidden and accessible based on user roles. Page-level security is implemented using access roles, row-level security, and slicers. A tooltip page shows a player's stats summary on the summary page. Power BI's new slicer is used to create captains' images in the slicer.

<h3>Key Explorations:</h3>
<ul>
  <li>Player Match Statistics: Analyzed the number of ODI and Test matches played by various players. Identified players with significant contributions in one format and minimal in another.</li>
  <li>Runs and Wickets: Investigated runs scored and wickets taken by players in both ODI and Test formats. Examined players with more than 1000 runs and 100 wickets in both formats.</li>
  <li>Test and ODI Captains: Reviewed the performance of Test and ODI captains, including their win percentages and contributions.</li>
  <li>Batting and Bowling Averages: Analyzed batting and bowling averages of key players across different formats.</li>
  <li>Historical Performance: Explored the number of debutants by year and notable historical achievements of Indian cricketers.</li>
</ul>

<h3>Insights:</h3>
<ul>
  <li>Player Contributions: Players like Sachin Tendulkar, Kapil Dev, and Anil Kumble have made significant contributions in both formats with high runs and wickets. These players are pivotal to India's cricketing history, highlighting their versatility and consistency.</li>
  <li>Match Statistics: Sachin Tendulkar has played the most ODI matches (463) and scored the highest number of runs. His long career and exceptional performance set a benchmark for future players.</li>
  <li>Bowling Performance: Anil Kumble and Kapil Dev have taken the highest number of wickets in Test matches. Their bowling prowess was instrumental in India's Test match successes.</li>
  <li>Batting Averages: Virat Kohli has one of the highest batting averages among current players, highlighting his consistency. Kohli's performance is critical for India's current and future cricketing success.</li>
  <li>Historical Debutants: The number of debutants has fluctuated over the decades, with notable peaks in certain periods. These peaks could correspond to strategic changes or the emergence of new talent in Indian cricket.</li>
</ul>
<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->

<h1>Credit Card Analysis</h1>

<h3>Objective:</h3>
To analyze credit card usage, customer demographics, and revenue metrics to identify key trends and areas for improvement. The goal is to optimize marketing strategies, develop targeted products, and enhance customer satisfaction.

<h3>Dashboard:</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/ash15h/Power-Bi-Dashboards/assets/67120563/27f4bd3d-a7a1-436d-bdfe-78ec8df13164" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/ash15h/Power-Bi-Dashboards/assets/67120563/b124075f-66d3-43fe-8678-d2b362b77c38" style="width: 80%; height: auto;">
</div>

<h3>Data Preparation:</h3>
<ul>
  <li>Removed Unnecessary Columns: Identified and removed columns not essential for the analysis.</li>
  <li>Handled Missing Data: Dropped rows with missing values to ensure data integrity.</li>
  <li>Removed Duplicates: Eliminated duplicate entries to maintain accurate results.</li>
  <li>DAX Measures: Used DAX to calculate weekly revenue, previous week revenue, week-over-week revenue, etc.</li>
</ul>

<h3>Key Explorations:</h3>
<ul>
  <li>Customer Demographics: Analyzed distribution by age, gender, income, education level, and job type.</li>
  <li>Revenue Metrics: Explored weekly and monthly revenue trends, revenue by expense type and payment mode, and total revenue by customer education level and job type.</li>
  <li>Credit Card Usage: Investigated customer numbers by card type (Blue, Gold, Platinum, Silver), customer satisfaction ratings, and activation rates within 30 days.</li>
  <li>Defaulters and Revolving Balance: Assessed the number of defaulters and total revolving balance by month.</li>
</ul>

<h3>Insights:</h3>
<ul>
  <li>Age Groups: Highest revenue from customers aged 31-50. Targeted marketing for these age groups is crucial.</li>
  <li>Job Types: Businessmen, white-collar workers, and self-employed contribute most to revenue. Customized products for these categories can boost satisfaction and loyalty.</li>
  <li>Education Level: Graduates and post-graduates generate the highest revenue. Promotions targeted at these groups can leverage their spending behavior.</li>
  <li>Gender: Further breakdown needed for precise insights. Gender-specific marketing could be beneficial.</li>
  <li>Monthly Revenue Trends: Peaks in certain months, drops in others. Understanding seasonal trends can optimize marketing activities.</li>
  <li>Payment Modes: Most revenue from chip and online payments. Enhancing these methods can increase usage.</li>
  <li>Defaulters: Monthly variation in defaulters. Mitigating factors can improve financial stability.</li>
</ul>

<h3>Recommendations:</h3>
<ul>
  <li>Targeted Marketing for Key Age Groups: Focus on 31-50 age groups to maximize revenue.</li>
  <li>Customized Credit Card Products: Offer specialized products for businessmen, white-collar workers, and self-employed individuals.</li>
  <li>Educational-targeted Promotions: Create promotions for graduates and post-graduates.</li>
  <li>Gender-specific Strategies: Develop gender-specific retention and acquisition strategies.</li>
  <li>Seasonal Marketing Plans: Align marketing plans with peak revenue months.</li>
  <li>Enhance Payment Methods: Improve chip and online payment experiences.</li>
  <li>Mitigate Defaulter Risk: Identify high-risk months and implement measures to reduce defaults.</li>
</ul>
<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->

<h1>Bank Churn Analysis </h1>

<h3>Objective:</h3> To analyze and predict customer churn by looking at factors like geography, gender, credit score, tenure, age, and salary. We used machine learning to calculate the churn probability of customers. The aim is to find ways to keep customers and reduce churn through practical insights.

<h3>Dashboard:</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/ash15h/Power-Bi-Dashboards/assets/67120563/a231fbcc-0406-43ef-aff8-d4fb437fe10a" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/ash15h/Power-Bi-Dashboards/assets/67120563/241b9365-3fc1-4722-9015-39293c0e77cc" style="width: 80%; height: auto;">
</div>

<h3>Data Preparation:</h3>
<ul>
<li> Removed unnecessary columns</li>
<li> Dropped rows with missing data</li>
<li>Encoded 'Geography' and 'Gender' using OneHotEncoder</li>
<li>Standardized features with StandardScaler</li></ul>

<h3>Modelling:</h3>
<ul>
<li>Trained a Random Forest classifier to predict customer churn</li>
<li>Added predicted churn probabilities to the dataset</li></ul>

<h3>Insights:</h3>
<ul>
<li>Geography: France has higher churn rates; service improvements are needed</li>
<li>Gender: More females are likely to churn</li>
<li>Credit Score: Lower scores correlate with higher churn, suggesting support services may help. Some high-score customers also churn, possibly seeking better services</li>
<li>Tenure: Shorter tenures correlate with higher churn, indicating better onboarding is needed</li>
<li>Age: Young adults and middle-aged customers show higher churn rates, needing targeted products</li>
<li>Salary: Middle-income customers and some high-income customers churn more, possibly due to service value perceptions</li>
</ul>

<h3>Recommendations:</h3>
<ul>
<li>Geographical Focus: Investigate why churn is high in France and improve services</li>
<li>Gender-specific Strategies: Develop tailored retention efforts for female customers</li>
<li>Credit Score Segmentation: Offer support for low-score customers and better options for high-score ones</li>
<li>Improving Onboarding: Enhance initial customer experiences to increase retention</li>
<li>Tailored Financial Products: Design products for younger and middle-aged customers</li>
<li>Competitive Pricing and Services: Review pricing and improve service value for middle-income customers</li>
<li>Credit Card Improvements: Upgrade credit card offerings to meet customer expectations</li>
</ul>
<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->
<h1>IPL Performance Analysis</h1>

<h3>Objective:</h3>
To analyze IPL matches, performance metrics, player statistics, venue statistics and historical data to identify key trends, top performers, and strategic insights for improving team performance

<h3>Dashboard:</h3> 

<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/ash15h/Power-Bi-Dashboards/assets/67120563/012f3d06-e4b1-49b2-8a9d-4a5fa4ac93b3" style="width: 80%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/ash15h/Power-Bi-Dashboards/assets/67120563/f86e32f3-a49b-40a2-8d66-d48739310750" style="width: 80%; height: auto; margin-bottom: 20px;">
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
  <img src="https://github.com/ash15h/Power-Bi-Dashboards/assets/67120563/b00d2564-e22c-4d01-9ea9-ea0e2f8a71de" style="width: 80%; height: auto; margin-bottom: 20px;">
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
<h1>Electoral Bonds Analysis (2019-2024 (Till May))</h1>

<h3>Objective:</h3> 
To analyse the data related to electoral bonds in India, focusing on the total denominations, political parties, purchasers, and trends over the years.

<h3>Dashboard:</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/ash15h/Power-Bi-Dashboards/assets/67120563/0fd9a1fb-141f-4e6e-ad92-0debafacc8de" style="width: 80%; height: auto; margin-bottom: 20px;">
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

<h1>Finance Analysis</h1>

<h3>Objective:</h3>To analyze the financial performance of the company from 2018 to 2020, focusing on key metrics such as sales revenue, gross profit, operational profit, PBIT (Profit Before Interest and Taxes), net profit, and EBITDA (Earnings Before Interest, Taxes, Depreciation, and Amortization). The aim is to identify trends, insights, and areas for improvement across all markets.

<h3>Dashboard:</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/ash15h/Power-Bi-Dashboards/assets/67120563/ab2f905e-d1d7-47ef-8664-a14fdbff20e6" style="width: 80%; height: auto; margin-bottom: 20px;">
</div>

<h3>Data Preparation:</h3>
<ul>
  <li>Removed Unnecessary Columns: Got rid of columns not needed for the analysis.</li>
  <li>Handled Missing Data: Dropped rows with missing values.</li>
  <li>Removed Duplicates: Cleaned up duplicate entries.</li>
  <li>Used DAX Measure: Calculated sales, gross profits, net profits, operational profit, PBIT, and EBITDA using DAX measures.</li>
  <li>Time Intelligence: Used time intelligence in DAX to calculate previous years' data for profits.</li>
</ul>

<h3>Key Explorations</h3>
<ul>
  <li>Profit Metrics: Checked gross profit, operational profit, PBIT, net profit, and EBITDA.</li>
  <li>Sales Data: Looked at total sales and gross profit by month and year. Also checked net profit by month and year.</li>
  <li>Yearly Profit Trends: Analyzed profit trends from 2018 to 2020 across different countries.</li>
  <li>Country-specific Performance: Looked at financial performance for each country, noting significant differences.</li>
</ul>

<h3>Insights:</h3>
<ul>
  <li>Gross Profit: Exceeded the goal by 34.59%, achieving €5.34M against a goal of €3.97M. This indicates strong sales performance and effective cost management overall.</li>
  <li>Operational Profit: Slightly above the goal by 3.15%, reaching €1.52M against a goal of €1.48M, showing operational efficiencies are in place but there's room for improvement.</li>
  <li>PBIT: Exceeded the goal by 4.7%, achieving €1.59M against a goal of €1.52M, reflecting good management of operating expenses.</li>
  <li>Net Profit: Slightly below the goal by 1.01%, reaching €1.29M against a goal of €1.30M, indicating effective overall financial management after accounting for all expenses.</li>
  <li>EBITDA: Exceeded the goal by 11.42%, achieving €2.24M against a goal of €2.01M, demonstrating strong earnings performance before accounting for interest, taxes, depreciation, and amortization.</li>
  <li>Sales Trends: Total sales to date amounted to €171,086,642, showing robust sales performance contributing significantly to gross profit.</li>
  <li>Country-specific Performance: Noticed financial loss in Australia. Sales revenue in Australia increased from 2018 to 2020, but the operational profit and net profit goals were not met. Despite strong sales, the financial losses highlight specific issues that need addressing to improve profitability in Australia.</li>
</ul>

<h3>Recommendations:</h3>
<ul>
  <li>Enhance Operational Efficiency: Keep improving processes to boost operational profit and hit net profit targets.</li>
  <li>Focus on Cost Management: Maintain strong cost management to ensure gross profit stays above targets.</li>
  <li>Monitor Trends: Regularly check monthly and yearly financial trends to spot and fix issues quickly.</li>
  <li>Country-specific Strategies: Create tailored plans for each country, especially to fix financial losses in Australia.</li>
  <li>Increase Sales Initiatives: Launch targeted sales efforts to further boost total sales and profitability.</li>
</ul>
<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->
