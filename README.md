# Predicting Increased Blood Pressure Using Machine Learning

## Topic and data characterization

In my project I tried to replicate the prediction of increased blood pressure by body mass index (BMI), waist (WC) and hip circumference (HC), and waist hip ratio (WHR) using a machine learning ([https://doi.org/10.1155/2014/637635](https://doi.org/10.1155/2014/637635)). Data were collected from 400 college students (56.3% women) from 16 to 63 years old.

## Aim

I wanted to build CART (Classification and Regression Tree) model. CART is a type of supervised learning technique for recursively partitioning a feature space into several parts (or nodes), based on the relationship between an outcome variable and one or more predictors. I compared the results from the CART analysis with traditional logistic regression analysis, in terms of strength of the prediction. Additionaly, I tried to use SVM and then CART model to improve analysis.

## Methods

The data were first split into two subsets, one for each sex. Then, each subset was randomly split into two sets (training and testing). I presented the data on different plots (2d and 3d). Then I balanced the data (this was not done in the publication). After data processing I preformed an analysis of both unbalanced and balanced data. Then I tried to use SVM and then CART on the balanced and unbalanced data.

## Preprocessing

- visualization
- balancing
- analysis of statistical parameters

## Accuracy

None of the models performed satisfactorily. It make sense because the given data do not form separate groups. The prediction was slightly better for female data. For men, if the data were not balanced, the models would not work properly. It also makes sense because male data were highly unbalanced (more than female data).

## Summary

Data connected with weight isn't good predictor of increased blood pressure alone. It could work better if we took into consideration other parameters like age, diet or genetics. The obtained results do not differ significantly from those in the publication. What is suprising, a pseudo r2 of 0.5 was satisfactory for the authors of publication. For me it is a very poor performance...
