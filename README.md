# deep-learning-challenge
![Alt Text}(https://github.com/lorigirton/deep-learning-challenge/blob/main/Red%20Black%20Circle%20Modern%20Kitchen%20Logo.png?raw=true)
## Overview
The purpose of this challenge was to create a tool that the fictional company, Alphabet Soup, could use to choose applicants to fund with the best chance of success. I designed a neural network to use the CSV data, containing information on more than 34,000 organizations that previously received funding from Alphabet Soup, to make predictions for future applicants.

## Results

### Data Processing

- **Target Variable:**
  - The target variable for this model is ‘IS_SUCCESSFUL’ because it is what I want the model to predict, indicating whether an applicant was successful (1) or not (0).

- **Features:** 
  - The features of this model include all the variables except the target variable ‘IS_SUCCESSFUL’, ‘EIN’ and ‘NAME’. These features are used as input for the neural network model.

- **Variables Removed:** 
  - ‘EIN’ and ‘NAME’ were removed from the input data because they were neither target variables nor features used for prediction.

### Compiling, Training and Evaluating

- **Number of Neurons and Layers:** 
  - I selected 80 neurons for the first hidden layer, 30 neurons for the second hidden layer, and 10 neurons for the third hidden layer. I chose these numbers through experimentation; increasing the numbers to 100, 50 and 10 did not significantly improve the accuracy. I used 3 hidden layers because it provided a balance between model complexity and performance. More or fewer layers resulted in decreased accuracy. 

- **Activation Functions:**
  - ReLU activation was used for the hidden layers due to its simplicity, efficiency and effectiveness in capturing complex patterns. For the output layer, I chose  sigmoid activation function because it is suitable for binary classification tasks. It squashes the output to a range between 0 and 1, representing the probability of an applicant being successful.
 
- **Attempts to Increase Performance:**
  - Experimentation with different optimization algorithms, but no significant improvement in accuracy was observed.
  - Increasing the number of hidden layers did result in a slightly better accuracy, although not significantly.
  - Handling the 'ASK_AMT' feature, focusing on applicants with an ask amount of $5,000, did not improve accuracy, regardles of filtering or retaining these records.
  - Modifying the number of neurons in the layers also did not yield a notable improvement in model performance.
 
## Summary
The overall results of this deep learning model showed limited improvement despite various attempts to optimize its performance. The model achieved an accuracy o fapproximately 72.5%, which indicates that it correctly predicts the success of applicants about 72.5% of the time. Although I made several attempts to enhance the model, such as adjusting the number of neurons, hidden layers, and optimization algorithms, the accuracy remained relatively stable. 

In the future, I would recommend exploring more sophisticated techniques or using different machine learning algorithms to solve this classification problem. Random Forest is one example I would like to try. Additionally exploring additional data sources could provide valuable insights for improving the prediction accuracy.
