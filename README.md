 Customer Churn Prediction

Project Objective  

The objective of this project is to “predict customer churn” in a telecom company using machine learning models.  
Customer churn refers to when a customer discontinues their subscription/service.  
By identifying at-risk customers, businesses can take “proactive retention measures” to reduce churn, optimize marketing strategies, and improve revenue stability.  

Project Workflow  

1. Data Understanding & Cleaning
      •	Loaded the dataset.
      •	Converted `TotalCharges` into numeric format and handled missing values.  
      •	Encoded categorical variables into numerical form.  

2. Exploratory Data Analysis (EDA)
      •	Checked churn distribution and confirmed dataset is highly imbalanced (majority of customers did not churn).  
      •	Explored relationships between churn and features like tenure, monthly charges, and internet service type.  

3. Model Building
      •	Split the dataset into training and testing sets.
      •	Trained a Decision Tree Classifier with depth and leaf constraints to avoid overfitting.  
      •	Applied SMOTEENN technique to handle imbalance by oversampling churned customers and cleaning noisy samples.  

4. Model Evaluation
      •	Accuracy was distorted by the imbalance.
      •	Focused on “precision, recall, and F1-score” especially for the churned class.  
      •	After applying SMOTEENN, there was a marked improvement in recall and F1-score for churn detection.

Key Insights Gained  

  a.	Imbalanced datasets require careful handling: Without balancing, the model missed many churned customers.  
  b.	Accuracy isn’t enough: Precision, recall, and F1-score provided better evaluation.  
  c.	SMOTEENN improved recall and helped detect more at-risk customers.  
  d.	Decision Tree Feature Importance revealed the strongest churn drivers.

Interpretation:

  a.	Customers with “shorter tenure” are more likely to churn.    
  b.	“Fiber optic customers” have higher churn compared to DSL/No service.  
  c.	Higher “monthly charges” and lower “total charges (newer customers)” also increase churn risk.  
  d.	Customers without internet service (and therefore streaming services) show lower churn rates.  

Business Actions Based on Insights  

Target at-risk groups for retention:
  a.	New customers with short tenure.  
  b.	Fiber optic internet users.  
  c.	Customers paying higher monthly charges.  

Retention Strategies:  

  a.	Offer “discounts or loyalty rewards” to new/short-tenure customers.  
  b.	Improve “Fiber optic service experience” to reduce dissatisfaction.  
  c.	Provide “bundled offers” to high-charge customers to increase perceived value. 
  d.	Monitor customer support interactions closely repeated complaints often signal churn risk.  




