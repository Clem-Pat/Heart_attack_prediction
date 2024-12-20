# Heart_attack_prediction
Academic project to study a medical database and predict heart attack risk using machine learning models. 

## Goal : 
- Access data of a Kaggle database
- Analyze data with Spark (like in Big Data situations)
- Train a Logistic regression model
- Train a Random Forest model
- Train a CNN ResNet 34 model
- Train a XGBoost model 

## Modules used : 
- Spark
- Scikit learn
- PyTorch

<a href="https://spark.apache.org/" target="_blank" rel="noreferrer">
  <img src="https://upload.wikimedia.org/wikipedia/commons/f/f3/Apache_Spark_logo.svg" alt="Spark" width="50" height="50"/>
</a>

<a href="https://scikit-learn.org/stable/" target="_blank" rel="noreferrer">
  <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" alt="Sklearn" width="50" height="50"/>
</a>

<a href="https://pytorch.org" target="_blank" rel="noreferrer">
  <img src="https://www.vectorlogo.zone/logos/pytorch/pytorch-icon.svg" alt="PyTorch" width="50" height="50"/>
</a>

## Summary

After accessing the data, we analyze it to understand the different features of the problem and the correlation between them. 
<br>
<img src="/Resources/output.png" alt="Age distribution in the dataset" width="500"/>
<br>
We checked for class balance; here, we can see that all age groups are well represented in the dataset. 

We can also observe the risk of being a victim of a heart attack depending on gender and tobacco consumption. 
<br>
<img src="/Resources/output1.png" alt="Heart attack risk depending on gender" width="500"/>
<img src="/Resources/output2.png" alt="Heart attack risk depending on tobacco consumption" width="500"/>
<br>

Then, we confirm the assessment that there is no correlation between the different features. 
<br>
<img src="/Resources/output3.png" alt="Heart attack risk depending on tobacco consumption" width="600"/>
<br>

Finally, we tried to train a logistic regression model, but it was overfitting. 
<br>
<img src="/Resources/output4.png" alt="Logistic regression model accuracy" width="600"/>
<br>

We then tried to train a random forest model, with various hyperparameters. Unfortunately, none of the solutions converged to a well-fitting training  
<br>
<img src="/Resources/output5.png" alt="Accuracy of random forest models" width="600"/>
<br>
Here, we observe that even with different tree numbers and tree depths, none of the models converged.


## Conclusion 
Finally we concluded that the dataset was too small to make any model converge: 
<br>
<img src="/Resources/output7.png" alt="Models accuracy" width="600"/>
<br>
This means that we cannot predict the heart attack risk using the patient features. 
In the next version of this study, we will use data augmentation to do oversampling. And we will try to train models to predict heart attack


## Authors

- [@Clem-Pat](https://www.github.com/Clem-Pat)
