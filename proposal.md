# Practicum Sprint 1
## Team Name
## Tentative Team Members & Roles
- Aheli Ghosh (aghosh314) - Backend(Node.js), frontend(HTML/CSS/react.js)
- Anirudh Prabakaran (aprabakaran3) - ML Engineer
- Harsh Goyal (hgoyal34) - Backend (Go) and ML Engineer
- Kanika Dhiman (kdhiman6) - Backend (Java + SpringBoot, APIs), Database
- Shivam Rustogi (srustgi3) -  Backend (Java + SpringBoot, APIs, Php (Hack), Python) 

## 1st Project Choice
### Topic
Diabetes Prediction App
### Project Type
End User Web Application
### Problem Summary
- Diabetes is a chronic disease where patients tend to have high levels of glucose in the blood, which can lead to serious health complications if not controlled properly. Type 2 Diabetes is the most common form of diabetes[1], which is often caused due to bad food habits and a sedentary lifestyle. According to the Centers for Disease Control and Prevention (CDC), more than 34 million people in the US have diabetes, and the number is expected to continue rising[2].  
- Diabetes has been one of the leading causes of death in the US[3], taking thousands of lives each year. It’s often accompanied by other life-threatening complications like heart disease, stroke, nerve damage, kidney disease and blindness[4]. Due to the high costs of treatment and pressure on the US healthcare system, public health efforts are focused on early detection and prevention, as well as better management of the disease[5]. This includes encouraging people to lead an active lifestyle, eating a healthy diet etc. In addition, there is even ongoing research into new treatments and cures for diabetes.  
### Proposed Solution
- There are many common diseases like Diabetes, which can be predicted with reasonable accuracy through healthcare analytics and Machine Learning. In this project, we plan to develop a web application, where we try to predict the chances of a user becoming diabetic in the future, given inputs like pregnancy info, BMI, age, insulin, gender, profession etc. 
- These are the tasks that we expect to complete sequentially:
  - Research on existing literature and try to understand how existing methods work. 
  - Curate datasets from multiple sources and do the necessary cleaning. 
  - Train our own models and compare performance with other off-the-shelf models. Assess which ones are more suitable for our application and finalize. 
  - Develop an API in Python, to expose the models as REST APIs in the FHIR standard. 
  - Develop a web application to expose these APIs, in a user-friendly user interface. 
### Potential Blockers (provide mitigation ideas if possible)
- Data Quality and Availability: Predictions may not be reliable if the data is incomplete, outdated or biased. 
- Privacy and Security Concerns: Since the user will be entering sensitive information, the web application must have the necessary security measures. 
- Model Bias: The data must represent the population well, if not it might develop a bias towards a certain gender, race etc. 
- Technical and UX challenges: This application requires expertise in multiple domains like Machine Learning, Web development, healthcare, security and so on. Integrating everything into an user-friendly application should be a challenging and interesting task. 

## 2nd Project Choice
### Topic
Stroke prediction and population management app
### Project Type
Pre-Defined Project type / End User Applications/Machine Learning
### Problem Summary
- According to the World Health Organization (WHO) stroke is the 2nd leading cause of death globally, responsible for approximately 11% of total deaths. Currently, stroke is the fifth leading cause of death and disability in the United States of America. Over 795k people in the US develop strokes every year, with about 610k of these being identified as the first or new stroke cases[6]. Moreover, deaths due to stroke account for about one of every twenty in the US. The US suffers an estimated loss of $34 Billion every year due to strokes which includes the cost of healthcare, lost income and productivity, and disability. 
- As highlighted by these statistics, stroke has a significant impact on individuals, families, and society as a whole, emphasizing the importance of efforts to prevent and treat stroke effectively.
### Proposed Solution
- We propose building a clinician-facing web application that can help predict the likelihood of a patient developing a stroke by analyzing the various health related attributes like age, bmi, smoke status, heart disease etc. We plan to utilize the Stroke Prediction dataset to build our machine learning model, with algorithms like Logistic regression to predict the risk score. The web application will provide the user with APIs that will help fetch the stroke risk score and identify high risk patients. Such an application would employ an ML model that continuously learns and improves its predictions, thus proving to be a valuable tool for ongoing stroke risk assessment and management. 
### Potential Blockers (provide mitigation ideas if possible)
- Incomplete Data: The available data for patients can be incomplete, and there may be significant variability in the way data is recorded, which can make it difficult to build accurate predictive models.
- Bias in the data: Data set may have imbalanced classes, which would yield inaccurate results. 
- Complexity: Making accurate predictions about which patients are at the highest risk of developing a stroke is important for early intervention and preventive care, but it is difficult because of the many variables involved and the complexity of the relationships between them. 
- Handling False Positives: While predicting stroke risk score, ideally we are permitted no margin of error as one prediction can lead to a wrong treatment and may prove fatal.

## 3rd Project Choice
### Topic
Real Time Claims using FHIR
### Project Type
End User Web Application
### Problem Summary
- Processing medical claims requires a lot of time, the billing system is slow, and the lengthy claims processing causes delays for providers as well. Because of this, transparency in price [2] and healthcare quality are impacted. Therefore, having a system that allows billing and is connected with claims processing based on the FHIR claim presented helps speed up choices such as helping providers know payment certainty and aiding payors in real-time estimation of claim settlement amounts, and more.
### Proposed Solution
- This project involves understanding the use cases related to searching and processing claims. The design aspect of the project involves creating a database in Base FHIR Claim format, as well as designing an API to process the claims for storage and to return the patient liability amount and payment covered by insurance. The claim adjudication process has two trigger points, which include the saving of a complete claim and a CRON (frequency determined by how frequently the data is uploaded). The user interface will have pages to search and store claims, as well as a page to display the Patient Liability amount and Payment Covered by Insurance.
### Potential Blockers (provide mitigation ideas if possible)
- Understanding the current billing and claims flow to structure the claim data which is needed to be stored.
- Use cases involved. Is it necessary to incorporate a billing system as well, which automatically fills up the claim data, or is it only sufficient to submit claim data, with claim adjudication then determining the patient liability amount and the payment covered by insurance?
- How does a Claim Adjudication take place? (for the prototyping)
- How do we retrieve the amount covered by a patient’s insurance?
- Data variability - the claims data could be present in several forms, which could lead to different structures. 

## References
1. Centers for Disease Control and Prevention. National Diabetes Statistics Report, 2020. 
2. American Diabetes Association. 
3. National Institute of Diabetes and Digestive and Kidney Diseases. Complications of Diabetes. 
4. American Diabetes Association. Fast Facts: Data and Statistics About Diabetes. https://www.diabetes.org/resources/statistics/statistics-about-diabetes
5. Centers for Disease Control and Prevention. National Diabetes Prevention Program. https://www.cdc.gov/diabetes/prevention/index.html
6. https://newsroom.heart.org/news/u-s-stroke-rate-declining-in-adults-75-and-older-yet-rising-in-adults-49-and-younger
7. Hospital Price Transparency - https://www.cms.gov/hospital-price-transparency 
