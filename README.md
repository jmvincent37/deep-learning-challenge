# Module 21 – Deep Learning Challenge

## Neural Network Model Analysis Report
### Overview of the Analysis
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. The purpose of this analysis is to develop a deep learning neural network model for a classification problem. The goal is to train the neural network to accurately classify instances into different classes based on the given features.

### Results 
#### Data Preprocessing:
• The target variable for the model is "IS_SUCCESSFUL".<br/>
•	The remaining features after deleting “EIN” and “NAME” were:
-	 APPLICATION_TYPE
-	 AFFILIATION
-	 CLASSIFICATION
-	 USE_CASE
-	 ORGANIZATION
-	 STATUS
-	 INCOME_AMT
-	 SPECIAL_CONSIDERATIONS
-	 ASK_AMT<br/>

#### Compiling, Training, and Evaluating the Model
1.	For optimization 1:
 -  Changed the cutoff value of the application type value counts from <10 to <500
 -	Changed the cutoff value of the classification value counts from <100 to <200
 -	Increased the number of hidden node layers from 2 to 3
 -	Increased the hidden node values for layers 1 & 2
 -	Changed the activation type from ‘relu’ to ‘leaky_relu’
 -	Increased the number of epochs from 100 to 125.
2.	For optimization 2:
-	Dropped “STATUS” feature
-	Changed the cutoff value of the classification value counts from <100 to <700
-	Increased the number of hidden node layers from 2 to 4
-	Increased the hidden node values for layers 1 & 2
-	Changed the activation type from ‘relu’ to ‘leaky_relu’
-	Increased the number of epochs from 100 to 150
3.	For optimization 3:
-	Dropped “STATUS” an “SPECIAL_CONSIDERATION” features
-	Changed the cutoff value of the application type value counts from <10 to <60
-	Changed the cutoff value of the classification value counts from <100 to <1000
-	Increased the number of hidden node layers from 2 to 4
-	Increased the hidden node values for layers 1 & 2
-	Changed the activation type from ‘relu’ to ‘leaky_relu’
-	Increased the number of epochs from 100 to 150
#### Summary
After several attempts at training the neural network to accurately classify instances into different classes based on the given features, the maximum accuracy achieved did not meet the .75 threshold. Based on research, increasing the data may have resulted in a better trained model. 

