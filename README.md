<h1>Bank Churn Analysis </h1>

<h3>Objective:</h3> To analyze and predict customer churn by looking at factors like geography, gender, credit score, tenure, age, and salary. We used machine learning to calculate the churn probability of customers. The aim is to find ways to keep customers and reduce churn through practical insights.

<h3>Dashboard:</h3>

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
- Geography: France has higher churn rates; service improvements are needed.
- Gender: More females are likely to churn.
- Credit Score: Lower scores correlate with higher churn, suggesting support services may help. Some high-score customers also churn, possibly seeking better services.
- Tenure: Shorter tenures correlate with higher churn, indicating better onboarding is needed.
- Age: Young adults and middle-aged customers show higher churn rates, needing targeted products.
- Salary: Middle-income customers and some high-income customers churn more, possibly due to service value perceptions.

<h3>Recommendations:</h3>
- Geographical Focus: Investigate why churn is high in France and improve services.
- Gender-specific Strategies: Develop tailored retention efforts for female customers.
- Credit Score Segmentation: Offer support for low-score customers and better options for high-score ones.
- Improving Onboarding: Enhance initial customer experiences to increase retention.
- Tailored Financial Products: Design products for younger and middle-aged customers.
- Competitive Pricing and Services: Review pricing and improve service value for middle-income customers.
- Credit Card Improvements: Upgrade credit card offerings to meet customer expectations.


