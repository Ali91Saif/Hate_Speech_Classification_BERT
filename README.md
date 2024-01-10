# Hate_Speech_Classification_BERT
In This Project, I have utilized the Dataset which contains Twitter data.
This was used to research hate-speech detection.
The text is classified as: hate-speech, offensive language, and neither. 
Due to the nature of the study, it’s important to note that this dataset contains  text that can be considered racist, sexist, homophobic, or generally offensive.

For this project, i have used Pre-Trained BERT Transformer Model for class prediction. I have performed FineTuning the Pre-Trained BERT Model from Hugging-face library and its implementation into MultiClass Classification Problem.

DataFrame Consists of 24783 data Instances (ROWS) accross 7 COLUMNS . However because of Computational Complexity which leads to 
large time consumption during training. i have decided to consider only 3000 data instances and used 2 epochs for Model training.

DataFrame contains Tweets and the classes in which they belongs. 
Cloumn Named 'class' contains multiple values,and they are label_encoded as:
0 -  signifies that the perticular Tweet has, neither a hate speech nor  a offensive language.
1 -  signifies that perticular Tweet is a Hate Speech.
2 -  signifies that the perticular Tweet has a offensive language.


Data set is splitted into training set and validation set, and this validation set is further sub-devided into test set.

Loss_Function used is 'Sparce Categorical Cross_Entropy'.
Optimizer used is 'Adam'. 
Learning_rate is kept at 5e-3 
Number_of_Epochs is set to 2

Model_Performance:

Even with this small training data and 2 epochs, this model has performed very satisfactorily, and was capable of capturing the information in
very efficient manner.

Model Accuracy Obtained with Test data is 85%. 
however , if the model is being trained on more data with more number of epochs,
It will definetly returns the better results. 
