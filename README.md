# TelcoChurn dataset using Scikit Learn.
Viability of Multi Layer Perceptron(MLP) Classifier to predict churn and K-means for customer clustering.

I greedily explore the viability of using a MLP to predict customer churn on the given dataset.
The final model has an accuracy of 80%.

Note: F1-Score for No is 87% and F1-Score for Yes is 60%. This shows a clear limitation of the MLP predicting who will in fact churn.

I attempt to cluster customers using KMeans and visualize the given clusters using Principal Component Analysis.
Note: The Kmeans model was not exposed to the 'Churn' column in the dataset.

# Insights
(1) : Due to inconsistent accuracy, MLP model is not ideal for this dataset. Recommended alternatives: Linear SVC, KNeighbours Classifier, SVC and finally Ensemble Classifiers. <br>
(2) : The clustering model places most of the churning customers together in one cluster. <br>
(3) : The profile of the cluster in (2) can potentially be defined with the following properties:<br />
  (a) No Device Protection<br />
  (b) No TechSupport<br />
  (c) Month-to-Month Contract Type<br />
  Hence we may forward these cluster properties to relevant people in marketing/business department to target<br /> 
  these types of customers to reduce churn. i.e Offer promotions and discounts to customers switching from month-to-month to 1-year and 2-year contracts.<br />
  
Note: The final visualization using pca with 3 components is an interactive plot inside the notebook.
