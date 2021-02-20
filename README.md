# Breast_Cancer_Detection-App

This application will detect **Breast-Cancer** .

The App Link :    https://breast-cancer-detection-ad-app.herokuapp.com/

Some Glimpses of Application : 

![rcd1](https://user-images.githubusercontent.com/61588604/108604652-35a27680-73d5-11eb-9760-f28c73e172ce.png)

![rcd2](https://user-images.githubusercontent.com/61588604/108604662-481cb000-73d5-11eb-8092-0e2c4c40fb99.png)

![rcd3](https://user-images.githubusercontent.com/61588604/108604680-5a96e980-73d5-11eb-9544-eb31e6d0996d.png)


Journey : 

**1) Data Collection** :  Data collecting process of thus project is AWESOME .

    a) used third party api and using python , "retrieve data of every day of every month of 2013-2018 year" from the html pages( web pages) of the BANGLORE Place .
    b)about data : Data Columns are : Average Temperature(T), Maximum Temperatre(TM), Minimum Temperature(Tm), Atmospheric Pressure at sea level (SLP), Average Relative Humidity(H) , Average Visibility, Average wind speed(V), Maximum sustained wind speed(VM), AQI-index ( PM 2.5 ) . 
    
    c) As a data scientist, we will predict the Air-Quality-Index for Banglore place, if user enter some features values as input .
    
    
**2) Data Preprocessing :** 
        
        a) checked the null values and removed those . 
        
        b) we collected data from 3rd party api using python so there were not many null values. All data is numerical .
        
        c) checked data that it is in guassian form. then scaled the data for some models (like linear , lasso, ridge...) because ensemble machine learning model don't need the scaled data .
        
        d) Now we can build machine learning models .
        
        

    
**3) Model building** : 

    a) split the dataset into X(independent features) and y(dependent features) .
    
    b) perform train_test_split .
    
    c) buoid models of -  linear regression,Lasso Regressor,Ridge regression , DecisionTreeRegressor, KNearestRegressor, RandomForestRegressor with hyperparameter tuning, XgBoost with hyperparameter tuning. 
    
    d) obsered that XGBoostRegressor with some parameters(got from hyperparameter tuning) has highest score and lowest error . so save this XgboostRegressor model using pickle.

**4) Model deployment** : 

    a) using flask framework , we deployed this model on HEROKU platform .
    
App link :  https://air-quality-prediction-app.herokuapp.com/
    
    

