# Breast_Cancer_Detection-App

This application will detect **Breast-Cancer** .

The App Link :    https://breast-cancer-detection-ad-app.herokuapp.com/

---->> Breast cancer is a dangerous disease for women. If it does not identify in the early-stage then the result will be the death of the patient. It is a common cancer in women worldwide. Worldwide near about 12% of women affected by breast cancer and the number is still increasing.

We have extracted features of breast cancer patient cells and normal person cells. As a Machine learning engineer / Data Scientist has to create an ML model to classify malignant and benign tumor. To complete this ML project we used the supervised machine learning classifier algorithms.

Some Glimpses of Application : 

![rcd](https://user-images.githubusercontent.com/61588604/108604706-8d40e200-73d5-11eb-815f-aa4958f6415b.png)

![rcd2](https://user-images.githubusercontent.com/61588604/108604715-9af66780-73d5-11eb-8765-09607ccf29d1.png)

![rcd3](https://user-images.githubusercontent.com/61588604/108604722-a6e22980-73d5-11eb-8446-257dcb0fb29c.png)


Journey : 

**1) Data Collection** :  Data is collected from seaborn_datasets .

    a)about data : dataset contains breast cancer patient cells and normal person cells . 
    
    b) As a data scientist, we will classify breast-cancer .
    
    
**2) Data Preprocessing :** 
        
        a) checked the null values and removed those . 
                
        b) checked data that it is in guassian form. then scaled the data for some models (like linear , lasso, ridge...) because ensemble machine learning model don't need the scaled data .
        
        c) Now we can build machine learning models .
        
        

    
**3) Model building** : 

    a) split the dataset into X(independent features) and y(dependent features) .
    
    b) perform train_test_split .
    
    c) buoid models of -  Logistic Regression , DecisionTreeClassifier, RandomForestClassifier with hyperparameter tuning, XgBoost Classifier with hyperparameter tuning. 
    
    d) obsered that XGBoost Classifier with some parameters(got from hyperparameter tuning) has highest score and lowest error . so save this XgboostRegressor model using pickle.

**4) Model deployment** : 

    a) using flask framework , we deployed this model on HEROKU platform .
    
App link :   https://breast-cancer-detection-ad-app.herokuapp.com/
    
    

