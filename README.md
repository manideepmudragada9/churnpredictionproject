# churnpredictionproject


  churn prediction project comprises of predicting churn from a realtime churn dataset of 25,000rows*111 columns.

  Dataset: 25,000*111 columns
  
  Tasks:-

          1.Data collection:-
                                 1.Data gathering 
                                 2.installaling jupyternotebook,libraries and importing them
                                 3.importing of dataset
                                 
          2. Data preprocessing:-
                                 1. removing missing value treatment
                                 2. removing null values
                                 3. removing duplicate records
                                 4.  removing unique value variables
                                 5.  removing zero variance columns
                                 6.  removing highly coorelated variables
                                 
         3.  outlier treatment:-
                                 1. Boxplot IQR method:- q3+(1.5*iqr)& q1-(1.5*iqr)
                                 2. standardisation :- +/-3 sigma approach
                                 3. Normalisation, capping and flooring.
                                 
        4.  Feauture extraction:-
                                 1. selecting feauture and target columns in variables 'X' & 'Y'
                                 2. spliting data into training and testing sets w.r.to 'X' & 'Y' and test size 25- 30 basing on the model and other parameters.
                                 
        5. Model selection:-    
                                 churn prediction is a classification problem as it needs a TRUE or FALSE / 0 & 1 as output so we will rely on 3 models.
                                                1. Decision Tree classsifer
                                                2. Random forest classifier
                                                3. Logistic Regression
                                 
        6. Model Building:-      
                                 1. Define model.
                                 2. Train model using fit() method :- 
                                                                       we will train model using x_train and y_ train. [model.fit(x_train,y_train)]
                                 
                                 3. Make Predictions on  the testing set :-
                                                                        we will make predictions on the x_test using model.predict(x_test) method
                                                                        
         7. Model Evaluation:- 
                                 1. Accuracy Evaluation :- we will evaluate accuracy using testing dataset and predicted dataset(y_test and y_predict)
                                                                with code:-     Accuracy_score(y_test,y_pred)
                                 2. Classification report :- we will evaluate precision,recall , f1-score and support  using  testing dataset and predicted dataset(y_test and y_predict)
                                                                with code:-  Classification_report(y_test,y_predict)
         
        8.  Hyperparametertuning :-  To increase accuracry we will try hyperparametertuning on the modified dataset.

                                 1. we define hyperparameters like :- 
                                                                      1. n_estimators
                                                                      2. max_depth
                                                                      3. min_samples_split
                                                                      4. min_samples_leaf
                                 2. train model again
                                 3.evaluate model
                                 4. adjust hyperparameters
                                 5. predict accurately  with the best hyperparameters found.



                                 



In this project, 
                  The best suited model is Random forest because of its effectiveness in  handle noise and missing values. Additionally, they are versatile and scalable, suitable for both classification and regression tasks. After evaluating all three models, we selected Random Forest due to its superior performance and minimal gap between training and testing accuracy
