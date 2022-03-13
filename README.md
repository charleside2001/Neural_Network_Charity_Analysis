 ![machine.png](https://github.com/charleside2001/Neural_Network_Charity_Analysis/blob/main/images/machine.png) 
# Overview of Neural Network Charity Analysis
The purpose of this project is to use `machine learning` and `neural networks` features to create a binary classifier that is capable of predicting whether job applicants will be successful if they are funded. 

To complete the task,  the following the following steps were completed using `CSV` dataset which contains more than `34,000` organizations that already received funding.

  * Preprocessing Data for a Neural Network Model
  * Compile, Train, and Evaluate the Model
  * Optimize the Model to see if predictive accuracy could be increased to over `75%`

## Results
  *1.*  Data Preprocessing
  
   *  IS_SUCCESSFUL is considered the target for this model?
        
   * Variables like APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and ASK_AMT are considered to be the features for this model?
        
   * Variables like EIN, NAME, STATUS, and SPECIAL_CONSIDERATION are neither targets nor features, and should be removed from the input data

  *2.* Compiling, Training, and Evaluating the Model
        
   #### 1st Attempt
   
   ![1st_attempt.png](https://github.com/charleside2001/Neural_Network_Charity_Analysis/blob/main/images/1st_attempt.png) 
   
   #### 2nd Attempt
   
   ![2nd_attempt.png](https://github.com/charleside2001/Neural_Network_Charity_Analysis/blob/main/images/2nd_attempt.png) 
   
   #### 3rd Attempt
   
   ![3rd_attempt.png](https://github.com/charleside2001/Neural_Network_Charity_Analysis/blob/main/images/3rd_attempt.png) 
   

   * At the end of this analysis, only `73%` accuracy was achieved even after optimizing the model to see if predictive accuracy could be increased to over `75%`
   * In order to increase model performance, I performed three attempts of the following steps
   
        * Removed noisy variables are removed from features
        * Added additional neurons  to hidden layers
        * Added additional hidden layers
        * Changed activation function of hidden layers
        * Saved  model's weights every `5 epochs`
        * Saved results to an `HDF5` file
  

## Summary 

Comparing the three model's predictive accuracy, their output is very similar, first attempt accuracy = `73.3%`, second attempt accuracy = `73%`, third attempt accuracy = `72.9%`. 

 #### 1st Attempt
   
     
  ![1st_accuracy.png](https://github.com/charleside2001/Neural_Network_Charity_Analysis/blob/main/images/1st_accuracy.png) 
   
 #### 2nd Attempt
   
     
  ![2nd_accuracy.png](https://github.com/charleside2001/Neural_Network_Charity_Analysis/blob/main/images/2nd_accuracy.png) 
   
 #### 3rd Attempt
   
     
  ![3rd_accuracy.png](https://github.com/charleside2001/Neural_Network_Charity_Analysis/blob/main/images/3rd_accuracy.png) 
   
   
Other predictive modeling approach like random forest could also be used to see if predictive accuracy could be increased to over `75%`. The decision-making process of whether to use a random forest versus a neural network will require further consideration/processing to be performed.

