 ## **Problem Definition:**

(Disclaimer: all information found here is _fictitious_) - CCD - Cardio Catch Diseases - is a company that offers services in **early diagnosys of cardiovascular diseases**. Currently a team of specialists is in charge of providing the diagnoses and the costs revolve around **RS1000 per diagnosys**. Customers are charged based on the diagnostic accuracy, ranging between **55% and 65%**. Each **5% increase in accuracy** levels above 50% costs **RS500 to the customer**. That results in fluctuating income for the company each month. Our job is to build a **cardiovascular disease classification model** that increases accuracy and precision of diagnoses that works with stable accuracy levels. 

### **_Business Problem Statement / Answers the CEO of the company is seeking:_**
- What are the values for precision and accuracy of the model?
- What is CCD's profit with this model?
- What is the confidence level of the model?

# **Solution Planning:**

### **Proposed Solution:** 
We're building a machine learning model that will **classify customers** based on their estimated probability of having some kind of cardiovascular condition. Model input will be a **set of features of each customers**. Ideally our model's precision level needs to be higher than 65%.  <br>
The model will be hosted on a cloud server so it can be **accessed remotely at any time** on [this website](https://fresmini-cardio.herokuapp.com/).

### **Project Walkthrough:**
- _Collecting data:_ all data is stored in a csv file;
- _Data description:_ check datatypes, null values and initial statistics;
- _Feature engineering:_ create business hypotheses and new features based on the original features;
- _Feature filtering:_ drop any non-helpful information;
- _Exploratory data analysis:_ dig deep into data to gather all possible information and attempt to validate our hypotheses;
- _Data preparation:_ get our data ready for machine learning models;
- _Feature selection:_ choose the most relevant features;
- _Machine learning models:_ train and compare several models and select the best performing ones;
- _Hyperparameter fine tuning:_ find optimal parameters for selected models and settle on the best one;
- _Business performance:_ evaluate how our model performs and answer the questions proposed by the CEO;
- _Model deployment into production:_ make our model available to the company.

# **Results Preview:**

![final ROC curve](https://user-images.githubusercontent.com/76906524/139515247-26e3ead6-ea77-4d59-850d-81ad52e6229a.png)

- Final model's **mean precision: 74.46%**. **Mean accuracy: 72.21%**. Mean recall: **68.64%** (even though it's not actually asked for, recall is an important metric in this context);
- CDD's **monthly profit**: **worst scenario: $176,000,00** - **best scenario: $264,000,00**
- The **confidence interval** is **0.76%** for a **99% confidence level**, which means that with 99% confidence the precision of the diagnosys is **within 73.70% and 75.21%**.

