# Predictive-model-for-customer-churn
Develop a predictive model for customer churn and provide actionable insights to minimize churn rates. Using historical customer data, we aim to identify the key factors influencing churn and recommend strategies to enhance customer retention.

# Data Overview

The dataset comprises customer information, consumption data, and various pricing metrics. Key features include:
	•	Consumption metrics (e.g., cons_12m, cons_last_month)
	•	Pricing variables (e.g., var_year_price_off_peak, var_6m_price_peak)
	•	Contract and customer engagement metrics (e.g., months_activ, months_to_end, tenure)
	•	Channel and origin information (e.g., channel, origin_up)
	•	Churn status (churn) and predicted churn probability (churn_probability)

# Methodology

	1.	Data Preprocessing:
	•	Cleaned and preprocessed data to handle missing values and categorical variables.
	•	Created new features such as cons_12m_segment based on consumption levels.
	•	Standardized numerical variables to ensure consistency across the dataset.
	2.	Exploratory Data Analysis (EDA):
	•	Generated histograms and density plots to understand the distribution of key variables.
	•	Plotted correlation matrices to identify relationships between features.
	•	Analyzed churn probabilities across different segments (e.g., price ranges, tenure).
	3.	Model Development:
	•	Implemented a Random Forest Classifier to predict customer churn.
	•	Evaluated model performance using accuracy, precision, recall, F1-score, and ROC-AUC.
	•	Improved model performance by addressing class imbalance using class weights and SMOTE (Synthetic Minority Over-sampling Technique).
	•	Explored alternative models like Gradient Boosting for enhanced performance.
	4.	Feature Importance and Interpretation:
	•	Identified key features influencing churn using feature importance scores.
	•	Visualized decision trees to understand the decision-making process of the model.
	5.	Churn Probability Analysis:
	•	Calculated churn probabilities for each customer using the best-performing model.
	•	Analyzed churn probabilities in relation to pricing metrics, tenure, and channels.
	•	Generated visualizations such as box plots and histograms to interpret the results.

# Key Findings

	1.	Churn Distribution:
	•	Majority of customers exhibit low churn probabilities, with a small subset at high risk.
	2.	Impact of Tenure:
	•	Churn probability decreases with longer tenure, indicating that newer customers are more likely to churn.
	3.	Pricing Sensitivity:
	•	Certain price ranges (e.g., 51-100, 251-300) show higher churn probabilities, suggesting critical pricing thresholds where customers become more price-sensitive.
	•	Higher price ranges (351-400, 400+) demonstrate lower churn probabilities, indicating that customers paying premium prices are less likely to churn.
	4.	Channel Influence:
	•	Different sales channels exhibit varying churn probabilities, with some channels showing higher risk. This suggests the need for targeted retention strategies based on the acquisition channel.

# Recommendations

	1.	Price Optimization:
	•	Reassess pricing strategies around critical thresholds (51-100, 251-300) to minimize churn.
	•	Reinforce value propositions for premium price segments to maintain low churn rates.
	2.	Customer Segmentation:
	•	Segment customers based on churn probability and tenure to implement targeted retention efforts.
	•	Focus on newer customers with higher churn probabilities for proactive engagement.
	3.	Channel Strategy:
	•	Develop customized retention plans for customers acquired through high-risk channels.
	•	Enhance customer experience and satisfaction across all channels to reduce churn.
	4.	Predictive Monitoring:
	•	Continuously monitor churn probabilities using the developed model to identify and address at-risk customers in real-time.
	•	Utilize insights from feature importance analysis to refine marketing and customer service strategies.

# Conclusion

By leveraging advanced machine learning techniques and detailed data analysis, this project provides a comprehensive understanding of customer churn dynamics. The insights and recommendations derived from this analysis can guide strategic decisions to enhance customer retention, optimize pricing, and improve overall business performance.
