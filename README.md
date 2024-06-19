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
<li>Added predicted churn probabilities to the dataset.</li></ul>

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
<h1>Bank Loan Analysis</h1>

<h3>Objective:</h3> To analyze customer demographics and loan data to identify trends and provide actionable insights for improving loan products and marketing strategies.

<h3>Dashboard:</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/ash15h/Power-Bi-Dashboards/assets/67120563/b00d2564-e22c-4d01-9ea9-ea0e2f8a71de" style="width: 80%; height: auto; margin-bottom: 20px;">
</div>

<h3>Data Preparation:</h3>
<ul>
<li>Removed Unnecessary Columns: Kept only columns relevant to the analysis.</li>
<li>Handled Missing Data: Dropped rows with missing values.</li>
<li>Removed Duplicates: Eliminated duplicate entries.</li>
</ul>

<h3>Data Analysis and Visualization:</h3>
<ul>
<li>Key Explorations:
  <ul>
    <li>Customer Demographics: Distribution of housing and other loans by age, job, and marital status.</li>
    <li>Loan Data: Monthly disbursement of housing and other loans, job-wise loan distribution, and loans by age and marital status.</li>
  </ul>
</li>
</ul>

<h3>Insights:</h3>
<ul>
<li>Age Groups:
  <ul>
    <li>Observation: 31-40 age group has the most housing loans; 19-30 age group prefers other loans.</li>
    <li>Implication: Target marketing for younger customers with specific loan products.</li>
  </ul>
</li>
<li>Job Categories:
  <ul>
    <li>Observation: Blue-collar and self-employed have the most housing loans; students and unemployed have the least.</li>
    <li>Implication: Customize loans for blue-collar and self-employed individuals.</li>
  </ul>
</li>
<li>Marital Status:
  <ul>
    <li>Observation: Married individuals take the most loans.</li>
    <li>Implication: Develop family-focused loan products.</li>
  </ul>
</li>
<li>Monthly Distribution:
  <ul>
    <li>Observation: May has the highest, December the lowest loan disbursements.</li>
    <li>Implication: Plan strategic marketing for peak months.</li>
  </ul>
</li>
</ul>

<h3>Recommendations:</h3>
<ul>
<li>Target Younger Demographics: Create loans for 19-30 age group inclined towards other loans.</li>
<li>Customize for Blue-collar and Self-employed: Offer loan products tailored to their needs.</li>
<li>Family-focused Loan Products: Introduce and market family-oriented loans.</li>
<li>Seasonal Loan Campaigns: Plan marketing campaigns during peak loan months (e.g., May).</li>
<li>Support for High-risk Jobs: Provide financial advice for customers in high-risk jobs to help manage loans better.</li>
</ul>
<hr style="border: 1px solid #fff; margin: 20px 0;">
<!------------------------------------------------------------------ End -------------------------------------------------------------------------->
