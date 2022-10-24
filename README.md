# Credit_Risk_Analysis

## Overview of the analysis: 

After learning skills in data preparation, statistical reasoning, and machine learning, now we had to solve a real-world challenge using machine learning: credit card risk. For this, we will employ different techniques to train and evaluate models with unbalanced classes using our skills in python to build and evaluate models using resampling.

We use the credit card credit dataset from LendingClub, a peer-to-peer lending services company, that we oversample the data and undersample using different techniques. Also, we use a combinatorial approach. Then, we build two machine learning models to reduce the bias to predict credit risk. Finally, we evaluate the performance of all the models we build to make a recommendation to predict credit risk. All the results we got from the models are describe in the next section.

### Results: 

In this section, we describe the balanced accuracy scores and the precision and recall scores of all six machine learning models:

-	**Naive Random Oversampling**, this model had a Balanced Accuracy of 64.4%, a Precision of 1% and a Recall of 69%. The results for the High-risk loans show us that this model has a high Recall, a low Precision for the risk loans and a F1 calculated of 0.02.

![Gráfica1](https://github.com/raulesqueda/Credit_Risk_Analysis-/blob/main/Images/grafica1.PNG)
 
-	**SMOTE Oversampling**, with this model the Balanced Accuracy results in 66.3%, with a Precision of 1% and a Recall of 63%. This model has better results with the Accuracy; however, this model is not the best to make a prediction.

![Gráfica2](https://github.com/raulesqueda/Credit_Risk_Analysis-/blob/main/Images/grafica2.PNG)
 
-	**Under sampling with Cluster Centroids**, the result of this model is not different than the two before, the Balanced Accuracy results in 54.4%, with a Precision of 1% and a Recall of 69%. This model has lower Accuracy, but a higher Recall, although, this model is not the best to make a prediction.

![Gráfica3](https://github.com/raulesqueda/Credit_Risk_Analysis-/blob/main/Images/grafica3.PNG)
 
-	**Combination (Over and Under Sampling)**, using the SMOTEENN algorithm, the results improved. The Balanced Accuracy results in 67.5%, with a Precision of 1% and a Recall of 76% and the F1 calculated results in 0.02, this result shows an unbalanced model that the previous one.

![Gráfica4](https://github.com/raulesqueda/Credit_Risk_Analysis-/blob/main/Images/grafica4.PNG)
 
-	**Balanced Random Forest Classifier**, with this algorithm the model statistics increased, the Balanced Accuracy results in 78.8%, with a Precision of 3% and a Recall of 70% and the F1 calculated results in 0.06. However, we have a low precision in this model.

![Gráfica5](https://github.com/raulesqueda/Credit_Risk_Analysis-/blob/main/Images/grafica5.PNG)
 
-	**Easy Ensemble AdaBoost Classifier**, this model has the best results of the estimated models, the Balanced Accuracy results in 93.2%, with a Precision of 9% and a Recall of 92% and the F1 calculated results in 0.16.

![Gráfica6](https://github.com/raulesqueda/Credit_Risk_Analysis-/blob/main/Images/grafica6.PNG)
 
### Summary: 

For the credit risk analysis, we develop a code using algorithms of machine learning, unfortunately, the models we estimate produce imbalance between the high-risk and low-risk credit data, this results in a biased models in any case.  However, this data could be useful to predict the low-risk credit than the high risk, this in terms of how many information the database has.

In this case, the use of oversampling and undersampling to improve the results of the models fails in the estimation of the models, the evaluation of the statistics of the models results in a lower Accuracy in the first four models; the last two models have an improve in terms of the statistics, however, but also fails in terms of predictions.

If we decided to use one model, the results of the Easy Ensemble Classifier had the best balance accuracy, precision, and recall of the 6 models analyzed, but we recommend to have more information and balanced information, to improve the power of prediction on any model. 
