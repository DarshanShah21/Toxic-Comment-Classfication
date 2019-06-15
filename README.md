# toxic-comment-classification
Given a text block, predict probability of toxicty for six different categories.

### Problem Statement
Given a comment from social media plattform, the task is to identify if it has any toxic content and classify it to belong to one or more of the following 6 categories toxic, severely toxic, obscene, threat, insult, and identity hate.

### Dataset
The dataset for this problem was obtained from Kaggle. Link to the dataset: https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/data

It contains Wikipedia talk page edits.
  - Train Set <br />
          ~150 thousand comments (68.8MB) <br />
          135 thousand labeled none (nontoxic), 15 thousand labeled toxic <br />
  - Test Set <br />
          ~100 thousand comments (60.4MB) <br />
        
Classes are imbalanced. Non-toxic comments contribute for almost up to 90% of the data and rest 10% are toxic.

### Models

##### Neural Network Models

1. Convolutional Neural Networks (cnn.ipynb)
2. A combination of Long Short Term Memory Networks and Convolutional Neural Networks (lstm-cnn.ipynb)

### Results 
It is a multi-label classification problem - As there are six different classes, one independednt model is developed for each class label and it is treated as a binary classification problem.
Simple accuracy is not a good measure since classes are imbalanced. Something like F1-score or balanced accuracy is a good reflection of model performance.
