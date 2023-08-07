# WiDS-Datathon-2020

## As part of a course in Data science, we were asked  to partcipate in an old competition in Kaggle.
In this task we were asked to present Shapley values, based on the results in Widsdatathon2020.
- We removed irrelevant columns with fixed values
- We removed columns with over 80% missing values
- Completion of missing values: we defined categorical and numerical columns - numerically we checked if the values
  are normally distributed or not and we filled in missing values ​​with the median or mean respectively. in columns
  Categorically, we replaced missing values ​​with the most common value.
- Normalization
- Division into bins

### We chose the Random Forest model which presented us with good results in work 1 and is of course based on an ensemble of Decision trees will therefore correspond with what we want to do in this work. We defined:
![image](https://github.com/Ilankorol1/WiDS-Datathon-2020/assets/103121260/9e3d6451-9c3c-43d7-8736-c633050abf35)

### We compared it with the base model and our model and here are the results:
![image](https://github.com/Ilankorol1/WiDS-Datathon-2020/assets/103121260/7111cb6e-7d7b-42bf-816e-fd59468d5e91)

### Analysis of Results :
- Both models are excellent in the training set, but the baseline model achieves the best results, with accuracy
Highest in all indices
- It can be seen that the evaluation results of the Train models are significantly higher than the evaluation results of
The test models. This is because the Train models are adjusted exactly to the training data, while the Test models are tested on
New data and not seen during training, which leads us to the next point -
- There is a problem of overfitting of both models. This can be seen from the large difference between the results obtained
between the training and testing sets. The model manages to successfully deal with the data it has already seen, but when
When new data arrives (such as in the test set), it has difficulty accurately predicting the result. If we were
Going back to work on the model, we would try to prevent overfitting by using an additional validation set, or a change
in the structure of the model itself.
- When you look at the Baseline model against the random forest, you can see that the evaluation results have
Positive correlation and absolutely similar.
- In a general and objective view, it can be seen that both models are not good enough to be used in practice, because they
show very low precision in the test set, which may lead to many wrong predictions.

## The model is random forest, we used TreeShap
![image](https://github.com/Ilankorol1/WiDS-Datathon-2020/assets/103121260/2ce90ab3-a667-416c-b02f-ac54182c64ed)
![image](https://github.com/Ilankorol1/WiDS-Datathon-2020/assets/103121260/50871669-8e2d-4cba-880a-3fe3b029610f)

## The baseline model is random forest, we used TreeShap and later also KarnelShap
![image](https://github.com/Ilankorol1/WiDS-Datathon-2020/assets/103121260/e0ebc489-ee12-4801-9293-9987ef39a690)
![image](https://github.com/Ilankorol1/WiDS-Datathon-2020/assets/103121260/acae80c8-40f5-4944-823c-81bc92522af2)



