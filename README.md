# Paypocket Data Analysis using Visualisation and Forecasting
### About: 
Paypocket payment analysis and estimated predictions using tools such as Python, PostgreSQL, PowerBI, Tableau, MS Excel and Jira.

![image](https://user-images.githubusercontent.com/89547823/165813130-ee026bec-4ec0-4261-8f58-7b1af9a920c1.png)

### Overview:
**Phase 1:** 
* 1.) Understanding business problem 
* 2.) Creating synthetic data

**Phase 2:** 

* 3.) Creating individual user story based visualisations and a compiled dashboard using PowerBI based on end user type (Payee and Payer)
* 4.) Creating time series forecasting and predictions using Python

**Phase 3:**
* 5.) Tool Evaluation (Tableau vs PowerBI)
* 6.) Project Management using JIRA

---
### Phase 1: Understanding business problem and creating synthetic data
![image](https://user-images.githubusercontent.com/89547823/165675876-9cce774a-883d-4813-baba-06d5dddcf453.png)

---
### Phase 2: Creating individual user story based visualisations
![image](https://user-images.githubusercontent.com/89547823/163530997-00a5b0f9-13b5-4d28-a44f-547a1f67fc28.png)

---
### Phase 2: Creating a compiled dashboard using PowerBI based on end user type (Payee and Payer)
![Paypocket Dashboard_Temp-1](https://user-images.githubusercontent.com/89547823/165676092-46a6056d-98a3-4796-8521-7f07431532ef.png)

---
![Paypocket Dashboard_Temp-2](https://user-images.githubusercontent.com/89547823/165676118-493299e5-5a6c-40da-9958-c3db0e1f9b66.png)

---
### Phase 2: Creating time series forecasting and predictions using Python

#### 1. Original Series
<img width="608" alt="Screen Shot 2022-04-27 at 8 48 50 PM" src="https://user-images.githubusercontent.com/89392789/165654444-504b9ecc-a8c0-4eb2-a745-4b6b6459b4b1.png">

#### 2. Stationarity test (Seasonal Components)
<img width="931" alt="Screen Shot 2022-04-27 at 8 49 42 PM" src="https://user-images.githubusercontent.com/89392789/165654525-0273ff50-ae9b-4747-b993-6eddebcf95df.png">

#### 3. Autocorrelation and Partial Autocorrelation Functions
<img width="924" alt="Screen Shot 2022-04-27 at 8 50 18 PM" src="https://user-images.githubusercontent.com/89392789/165654582-e8e7e2e8-7130-427d-b445-8f582ff1b8ad.png">

#### 4. Loess Smoothing
<img width="725" alt="Screen Shot 2022-04-27 at 8 50 49 PM" src="https://user-images.githubusercontent.com/89392789/165654627-402bd7c6-ab0c-4cf9-a6a7-b3298336398e.png">

#### 5. Simple Exponential Smoothing
<img width="386" alt="Screen Shot 2022-04-27 at 8 51 14 PM" src="https://user-images.githubusercontent.com/89392789/165654666-d384ad79-1ac2-49db-9a36-dea984fdd409.png">

* **Results:**
The Series is already smooth for the given dataset so, smoothening is not required.

#### 6. Stationarity test
**Results:**
* **ADF Test Statistic :** -0.99916608535741
* **p-value :** 0.7535683308711256
* **Number of Lags Used :** 12
* **Number of Observations :** 431

Weak evidence against null hypothesis,indicating it is Non-Stationary 

#### 7. First order difference
<img width="422" alt="Screen Shot 2022-04-27 at 8 53 19 PM" src="https://user-images.githubusercontent.com/89392789/165654851-4eb7c831-613f-4653-89fc-d12ef43bd8ff.png">

* **Autocorrelation and Partial Autocorrelation Functions of Differenced Series**
<img width="772" alt="Screen Shot 2022-04-27 at 8 53 44 PM" src="https://user-images.githubusercontent.com/89392789/165654900-878137ff-c3c6-48bd-8dfa-f1ce7cc906ec.png">

#### 8. SARIMAX model of order (1,2,1)
<img width="721" alt="Screen Shot 2022-04-27 at 8 54 42 PM" src="https://user-images.githubusercontent.com/89392789/165654993-2f4dfb91-525b-4808-84b9-6e915d3d7f9a.png">

#### 9. ARIMA model of the order (2,0,3)
<img width="767" alt="Screen Shot 2022-04-27 at 8 55 41 PM" src="https://user-images.githubusercontent.com/89392789/165655071-3387336a-4d1e-49b2-a40d-fcf850340572.png">

#### 10. Encoding of data with two different techniques:
**i.) One hot encoding :**
Accuracy: 64.63%

**ii.) Ordinal encoding :**
Accuracy: 67.35%
 
 #### Results: 
 On our dataset, Ordinal transform gives better results than One hot encoder.
 
---
### Phase 3: Tool Evaluation (Tableau vs PowerBI)
![image](https://user-images.githubusercontent.com/89547823/165814460-440dcc48-6271-405b-811f-e075629993bd.png)

**Final Recommendation: Tableau**

---
### Phase 3: Project Management using JIRA

* Transparency
  * Sprints, status roadmap, backlog
* Collaboration
  * Effective utilization of comment section
* Accountability 
  * Assigning tasks, due dates
* Integration
  * Google Drive and documentation

---
