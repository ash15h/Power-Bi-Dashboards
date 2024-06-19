<h1>Bank Churn Analysis </h1>
<h3>Objective:</h3> To analyze and predict customer churn by looking at factors like geography, gender, credit score, tenure, age, and salary. We used machine learning to calculate the churn probability of customers. The aim is to find ways to keep customers and reduce churn through practical insights.
<h3>Dashboard:</h3>
<div style="width: 100%; text-align: center; margin-bottom: 20px;">
  <img src="https://github.com/ash15h/Power-Bi-Dashboards/assets/67120563/f3939f99-b974-4c1a-8d38-8058ed6dc129" style="width: 100%; height: auto; margin-bottom: 20px;">
  <img src="https://github.com/ash15h/Power-Bi-Dashboards/assets/67120563/241b9365-3fc1-4722-9015-39293c0e77cc" style="width: 100%; height: auto;">
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


