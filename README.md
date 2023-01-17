# Supervised_ML_Heart_Disease
In this project I used classification models to predict heart disease based on patient data. Furthermore, the project was presented to a fictional hospital board (other students at a coding bootcamp) with a focus on developing a better scoring to maximize model performance on.

The logic of the selection of scoring measure was that telling a patient with a heart disease that they are healthy is worse than the opposite, since sending a ill patient home could result in death. Based on this, I maximized the the different models based on recall, and got a logreg model with a 97.5% recall score after hyperparameter tuning.

However, a key thing that is missing in this reasoning is money, i.e. the cost of treating a healthy patient due to misclassification in the model (the True Negatives). My proposition to this fictional board was the develop a new scoring method where both False Positives and True Negatives where taken into consideration. As you might have guessed by now, we already have this score built in to most (if not all) ML-classification models, namely accuracy. The problem with accuracy in my case is that it weighs FP and TN equally important, which I argue is not the case. I argue that not sending home ill patients and risking their lives (minimizing FP) is more important than minimizing the cost of treating healthy ones (minimizing TN). 

This project had a large focus on storytelling in the presentation and building a case to present to a non-ML knowing crowd. 

