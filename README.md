# Credit Risk Analysis


## Overview
The following report uses statistical reasoning, and machine learning to assist in classifying the credit risk into good loans and risky loans based on a Data Set from LendingClub. The Data was sampled using a variety of algorithms and models including: RandomOverSampler, SMOTE, ClusterCentroids, BalancedRandomForestClassifier, EasyEnsembleClassifier. These are evauated below to determine if they are effective to predict credit risk.

## Results

### RandomOverSampler

![ROS_BAS](https://user-images.githubusercontent.com/90511014/155633409-c7f1865f-3b31-4544-84e9-ea8321db6fb1.png)

![ROS CM](https://user-images.githubusercontent.com/90511014/155633429-6f985999-ee5b-4f71-8631-61694180ec86.png)

![ROS ICR](https://user-images.githubusercontent.com/90511014/155633435-c699a314-5d54-45e2-a458-2d0e7aae827e.png)

- The balanced accuracy score is 0.67.
- The precision score for high-risk is 0.01.
- The recall score for high-risk is 0.74.
- The precision score for low-risk is 1.00.
- The recall score for low-risk is 0.61.


### SMOTE

![SMO BAS](https://user-images.githubusercontent.com/90511014/155633448-5b2dbac2-b87e-4070-a7eb-31a43e16d81c.png)

![SMO CM](https://user-images.githubusercontent.com/90511014/155633463-fefa0775-f1e2-4f20-97df-2175396b05db.png)

![SMO ICR](https://user-images.githubusercontent.com/90511014/155633471-c42f85f2-b43a-4e59-9f09-db8670642572.png)


- The balanced accuracy score is 0.66.
- The precision score for high-risk is 0.01.
- The recall score for high-risk is 0.63.
- The precision score for low-risk is 1.00.
- The recall score for low-risk is 0.69.

### ClusterCentroids

![CC BAS](https://user-images.githubusercontent.com/90511014/155633597-529c668b-9754-4355-bbeb-e6013d9793ce.png)


![CC CM](https://user-images.githubusercontent.com/90511014/155633580-39e25974-ee9c-48a9-be7a-3381e0ea03b4.png)

![CC ICR](https://user-images.githubusercontent.com/90511014/155633586-3af8f1d7-c8ad-49e0-9ea8-15da03a7aff2.png)


- The balanced accuracy score is 0.54.
- The precision score for high-risk is 0.01.
- The recall score for high-risk is 0.69.
- The precision score for low-risk is 1.00.
- The recall score for low-risk is 0.40.




### SMOTEENN

![EEN BAS](https://user-images.githubusercontent.com/90511014/155633620-2a9c669a-002f-426d-995d-4bec795ff903.png)

![EEN CM](https://user-images.githubusercontent.com/90511014/155633641-20ba1a36-91fd-4440-9da8-8a54aaab46aa.png)


![EEN ICR](https://user-images.githubusercontent.com/90511014/155633645-a15c87bf-03e9-4657-857d-d2328f0bdda5.png)

- The balanced accuracy score is 0.54.
- The precision score for high-risk is 0.01.
- The recall score for high-risk is 0.73.
- The precision score for low-risk is 1.00.
- The recall score for low-risk is 0.59.

### BalancedRandomForestClassifier

![BRF BAS](https://user-images.githubusercontent.com/90511014/155633665-849f5d8d-de15-454f-be68-249720069fae.png)


![BRF CM](https://user-images.githubusercontent.com/90511014/155633672-fa8a41ac-8998-49b6-8b9e-73ab389f2eac.png)


![BRF ICR](https://user-images.githubusercontent.com/90511014/155633677-1e565f7a-9107-4b31-b739-0bed6a406418.png)


- The balanced accuracy score is 0.79.
- The precision score for high-risk is 0.03.
- The recall score for high-risk is 0.70.
- The precision score for low-risk is 1.00.
- The recall score for low-risk is 0.87.



### EasyEnsembleClassifier

![EEC BAS](https://user-images.githubusercontent.com/90511014/155633689-6d87f47c-51c5-4809-81b3-2e28085d05bf.png)

![EEC CM](https://user-images.githubusercontent.com/90511014/155633722-b913faf7-0bfa-47f2-a94a-6a552b710c31.png)

![EEC ICR](https://user-images.githubusercontent.com/90511014/155633737-58844fa4-f591-43bc-8120-082214822dba.png)

- The balanced accuracy score is 0.92.
- The precision score for high-risk is 0.05.
- The recall score for high-risk is 0.93.
- The precision score for low-risk is 1.00.
- The recall score for low-risk is 0.90.

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.
## Summary

Summarize the results of the machine learning models, and 
- EasyEnsembleClassifier had the highest balanced accuracy score at 0.92
- SMOTEENN and ClusterCentroids had the lowest balanced accuracy score at 0.54.
- EasyEnsembleClassifier had the highest high-risk precision at 0.05
- The others except for BalancedRandomForestClassifier had the lowest high-risk precision at 0.01.
- EasyEnsembleClassifier had the highest high-risk recall at 0.93.
- SMOTE had the lowest high-risk recall at 0.63.
- Each model had a the same low-risk precision score at 1.00.
- EasyEnsembleClassifier had the highest low-risk recall at 0.90.
- ClusterCentroidshad the lowest low-risk recall at 0.40.

To have the best return on investment It would be more important to not loan to high risk rather than potentially reject a good loan. However there still needs to be enough good loans available. 

include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
