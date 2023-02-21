# COVID-19-Vaccination-Likelihood
SRS Case Study: The goal is to understand a person's chances of getting the COVID-19 Vaccine. 

Interpreting the model's relevant performance metrics.
This study focuses on how a persons environment and beliefs affect their willingness to take the COVID-19 vaccine. People bear several reservations, but overall suervey sample population show inclination towards getting the COVID-19 vaccine. Geographic locations (FIPS, ZIP, State), Median household income, Education, Age, Race and Trust (on goverment, Scientists) appears to be the key determinants of vaccination intent. Among others, beliefs and personal experiences are ranked higher within Random Forest model. This study intends to estimate what drives the perception of the masses towards COVID-19 vaccination. Six models, e.g., Naive Bayes, random forest (RF), a support vector machine (SVM), decision tree (DT), K-nearest neighbor (KNN), and eXtreme Gradient Boosting (XGboost), were used for forecasting the overall predilection toward the COVID-19 vaccine. A voting classifier was used at the end of this study to determine the accuracy of all the classifiers. The results prove that the SVM and Logit model after hyperparameter tuning produces the best forecasting results (accuracy: 52%) and that KNN (accuracy: 52%) did not improve much after tuning and produced the worst prediction toward the intent to be vaccinated by the COVID-19 vaccine. When using the voting classifier, the proposed system provided an overall accuracy of 56%.

Thus, the results show that the studied prediction technique is a promising, with improvements feature engineering and additonal supporting data to propose coverage-enhancing policy responses.

# Recommendation regarding putting the model in production and How should it be used?

In my opinion, having a model with consistently good performance (at least 80% or more -accuracy/f1 score) is essential for production. As the metrics show that the current model is not performing well (accuracy obtained after tuning SVC: ~59%), I would not recommend putting the model in production.  

Without consistent performance, we will not be able to set up the tests to determine if the model is behaving as expected. I recommend improving the current model by adding new data, thorough feature engineering, and parameter tuning. 
