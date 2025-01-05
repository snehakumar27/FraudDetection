# Fraud Detection
The main work has been done in `Fraud_Detection.ipynb'. Python 3.11.5 has been used in this project. Additional files: 
- `saved_objects` folder : contains saved states of all the models. Please unzip the file and keep it in the same working directory as this notebook 
- `autoencoder_tuning` folder : contains the trials for autoencoder. Please unzip the file and keep it in the same working directory as this notebook 
- `requirements.txt` : list of libraries from the python environment used while running this notebook.

## Background & Motivation  
With the rapidly evolving capabilities of technology, financial fraud has emerged as one of the prevalent issues in the recent years. Whether through online banking, e-commerce platforms or credit cards, financial scams and fraud are become increasingly sophisticated and pervasive. In Singapore, scam victims lost over $380 million in just the first half of 2024, with scam cases increasing by 16.3% ([Sun, 2024](https://www.straitstimes.com/singapore/scam-victims-in-s-pore-lost-3856m-in-first-half-of-2024-as-number-of-cases-hit-high-of-26587)). Globally, 17% rise in digital fraud attacks in financial services has been reported ([Fintech News Singapore, 2024](https://fintechnews.sg/101575/regtech/fraud-attacks-financial-services-payment-account-creation-fraud/)). Detecting fraud has become more critical to safeguard individuals and prevent financial losses. With this motivation, I decided to explore what are the ways in which machine learning could be applied in detecting fraudulent transactions. While there are many forms of financial fraud, for the purposes of this project, we will be focusing only on credit card fraud. 

## Project Goal 
In the context of machine learning, the problem of fraud detection can be formulated in two different ways: 
1)	**Classification Problem**: A supervised learning task (binary classification), where given a set of input variables, the model would classify the transaction as normal or fraudulent. 

2)	**Anomaly Detection**: An unsupervised learning task, where common patterns of normal transactions are learnt by the model and use to identify data points that significantly deviate from these patterns as anomalies. The task can also be viewed as semi-supervised as data labels are used to guide in obtaining an optimal decision threshold for labelling anomalies. 

**The goal of this project was to compare these two formulations and determine which of them a) results in better perfomrnace & b) provides a better representation of the credit card fraud detection task.** 
