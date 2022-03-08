# Plant-Disease-Classification
Detection of disease in plants using CNN algorithm

The model is built based on Teacher-Student Architecture, Which consists of three classifier Teacher, Decoder and Student Classifier

Teacher and Student classifiers use VGG-16 Architecture which are loaded with the weights of the model trained on Image Net Dataset(Which is known as Transfer Learning).

Using transfer learning decreases the computational complexity and also increases the accuracy

The dataset used is publicly available Plant Village Dataset

The above model provides a better visual view of the infected parts of plants, Which can be seen in the below image!
![Visual view](https://user-images.githubusercontent.com/74169520/157288145-b7822172-46eb-432f-af98-3160daea751f.jpg)

The output from the Teacher classifier is used as input for the decode classifier whose output is the visual view shown above, Later this image is used as input for the student classifier for training.
![Teacher Student Model](https://user-images.githubusercontent.com/74169520/157288180-05eaf556-0b42-49a1-998b-c2c2f8d16040.jpg)

The above .ipynb file contains the code for building the model, training it and saving the weights

We have used the accuracy metric for measuring the model

The loss function used is Categorical Cross-Entropy Loss which is used for tasks where we are classifying more than two categories else Binary Cross-Entropy Loss can be used.

You could check out the code in the file Plant Disease Classification

The above model is built using the reference as provided below.

Reference
