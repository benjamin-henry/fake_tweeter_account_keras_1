# fake_tweeter_account_keras_1

# Info
From https://github.com/NikhilCodes/Fake-Twitter-Account-Detection-Keras and https://paperswithcode.com/paper/fame-for-sale-efficient-detection-of-fake/review/

Datasets used (cleaned in https://github.com/NikhilCodes/Fake-Twitter-Account-Detection-Keras):
- Elezioni2013
- Intertwitter

legit accounts : 1481 / fake accounts  : 1337

# results
train_and_eval_1:
- 64% of dataset for training data
- 16% of dataset for validation data
- 20% of dataset for test data (not seen during training)
- test loss : 0.017
- test accuracy : 99.29%
- confusion matrix : \
&emsp legit  [295 ,   2]\
&emsp fake   [  2 , 266]\
&emsp legit, fake
- model: ".model/classifier_1.h5"

train_and_eval_2 (based on https://github.com/NikhilCodes/Fake-Twitter-Account-Detection-Keras/blob/master/trainer_and_solver.ipynb):
- 76% of dataset for training data
- 24% of dataset for validation data
- loss : 0.037
- accuracy : 99.85%
- confusion matrix :
    legit  [358 ,   0],
    fake   [  1 , 318]
           legit, fake
- model: ".model/classifier_2.h5"
