# Insurance-Prediction
Deep Learning model with Kaggle Dataset

## Health Insurance Cross Sell Prediction

### Description: 
Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

reference : https://www.kaggle.com/datasets/anmolkumar/health-insurance-cross-sell-prediction?select=sample_submission.csv

### Dataset Variables Definition

| Variable   |      Definition      |
|----------|:-------------|
| id |  Unique ID for the customer |
| Gender |    Gender of the customer   |
| Age | Age of the customer |
| Driving_License |   0 : Customer does not have DL, 1 : Customer already has DL  |
| Region_Code | Unique code for the region of the customer |
| Previously_Insured |   1 : Customer already has Vehicle Insurance, 0 : Customer doesn't have Vehicle Insurance
| Vehicle_Age	 | Age of the Vehicle|
| Vehicle_Damage |  1 : Customer got his/her vehicle damaged in the past. 0 : Customer didn't get his/her vehicle damaged in the past.  |
| Annual_Premium | The amount customer needs to pay as premium in the year |
| Policy_Sales_Channel |    Anonymized Code for the channel of outreaching to the customer ie. Different Agents, Over Mail, Over Phone, In Person, etc.   |
| Vintage |Number of Days, Customer has been associated with the company |
| Response | 1 : Customer is interested, 0 : Customer is not interested |

### Model Detail

- Neural Network Model (Linear -> Tenh -> Linear -> Regression) with Logistic Regression for Classification Class
- Features Selecting with chi2 Dependent Testify of sklearn - SelectBestK 
- Hyperparameters optimization with Optuna - Tree Parzen Estimator (based on Bayesian) method
- Adam Optimization, BCELoss
- AUC to be the evaluation method

#### Built with Pytorch
