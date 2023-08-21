## PWC-customers-retention-dashboard

# Table of Content:
+ Problem Statement
+ Data Source
+ Data Preparation
+ Data Visualization
+ Insight


# Problem Statement:
+ Define proper KPIs
+ Create a dashboard for the retention manager reflecting the KPIs

# Data Source:

# Data Preparation:
+ Data transformation was done in power query editor then loaded dataset into power bi desktop

+ Created some measures using DAX that are:
  - Total Customers = `COUNT('01 Churn-Dataset'[customerID])`
  - Churned Customer = `COUNTX(FILTER('01 Churn-Dataset' , '01 Churn-Dataset'[Churn] = "Yes") , '01 Churn-Dataset'[customerID])`
  - Churn rate = `'01 Churn-Dataset'[Churned Customer]/'01 Churn-Dataset'[Total Customers]`
 
# Data Visualization: 

![Customer retention 1](https://github.com/Ananya-Foujdar05/PWC-customers-retention-dashboard/assets/140806083/2c176ec7-783c-4a90-b670-be1ea83b2049)

![Customer Retention 2](https://github.com/Ananya-Foujdar05/PWC-customers-retention-dashboard/assets/140806083/ea5a0235-914c-4752-89c9-7a5b680eaea9)

# Insights:
As we can conclude
+ There are 1869 churned customers which are 26.54% of total customers
+ female customers show a higher churn rate compared to male customers, highlighting the importance of targeted retention strategies.
+ Month-to-month contracts exhibit a higher churn rate than longer-term commitments, emphasizing the need for enhanced engagement throughout the customer journey.
+ Fiber optics customers demonstrate a higher churn rate compared to DSL or no internet connection users. Understanding the impact of technology preferences is key.
+ Unsurprisingly, customers without tech support are more prone to churning. Addressing their concerns promptly is pivotal to ensuring their loyality.
+ the churn rates for customers with or without multiple lines are strikingly similar. This insight sparks intriguing questions about the factors driving their decisions.
+ Customers without device protection display a higher churn rate, signaling an opportunity to enhance protection offerings and build lasting trust.
+ Non-streamers are more likely to churn compared to active streamers. Crafting tailored content experiences could be a retention game-changer.
+ Customers lacking online backups exhibit a higher churn rate. Strengthening data protection measures could be pivotal in their retention journey.


