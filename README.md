# fake_tweeter_account_keras_1

# Warning
Please, do not use it for real purposes. I mean I don't know if I would use it if I wanted to buy the blue bird. 

# Info
From https://github.com/NikhilCodes/Fake-Twitter-Account-Detection-Keras and https://paperswithcode.com/paper/fame-for-sale-efficient-detection-of-fake/review/

# Data
Datasets used (cleaned in https://github.com/NikhilCodes/Fake-Twitter-Account-Detection-Keras):
- Elezioni2013
- Intertwitter

legit accounts : 1481 \
fake accounts  : 1337 ;) \
total : 2818

Used to build training data:
- user has an url ? 1 if true, else -1
- user's profile is default profile ? 1 if true, else -1
- profile has a description ? 1 if true, else -1
- friends over followers ratio 
- profile has favourites ? 1 if true, else -1
- profile listed ? 1 if true, else -1

# Results
train_and_eval_1:
- 64% of dataset for training data
- 16% of dataset for validation data
- 20% of dataset for test data (not seen during training)
- test loss : 0.083
- test accuracy : 99.11%
- confusion matrix : \
     legit     [294 ,   3] \
     fake      [  2 , 266] 
- model: ".model/classifier_1.h5"
