## SMS Spam Detection using Naive Bayes
# Introduction
This project uses a Machine Learning approach to classify SMS messages as either spam or not spam. It employs the Naive Bayes algorithm—a probabilistic machine learning model well-suited for text classification tasks. The dataset used is the SMS Spam Collection from the UCI Machine Learning Repository, which contains 5,574 SMS messages labeled as spam or ham (not spam).

Dataset
The dataset used for this project is the SMS Spam Collection, which is available publicly on the UCI Machine Learning Repository.

Dataset citation: Almeida, T. & Hidalgo, J. (2011). SMS Spam Collection [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5CC84.
The dataset consists of two columns:
label: indicates whether the message is "spam" or "ham" (not spam)
message: the content of the SMS message

Features
Text Preprocessing: We use CountVectorizer to convert the text messages into a bag-of-words model, which is essential for training the Naive Bayes classifier.
Naive Bayes Classification: The model used for this project is Multinomial Naive Bayes, a widely-used algorithm for text classification tasks.
Prediction: The project includes functionality to predict if a new message is spam or not by inputting any new message.
Project Structure
smsspamcollection/ – Contains the dataset file (SMSSpamCollection).
sms_spam_detection.py – The Python script that trains the model and provides functionality for predicting a new message.
README.md – The description and documentation of the project.
requirements.txt – The Python libraries required to run the project.
Prerequisites
To run this project, ensure that you have the following installed:


Required libraries:
pandas
scikit-learn
requests
zipfile

You can install the required libraries by running:



pip install -r requirements.txt
Instructions to Run the Project

Step 1: Clone the Repository
To get a copy of the project up and running on your local machine:
git clone https://github.com/your_username/sms-spam-detection.git
cd SMS_Spam-Prediction

Step 2: Download and Load the Dataset
The script automatically downloads and loads the dataset from the UCI Machine Learning Repository. You do not need to manually download the dataset.

Step 3: Run the Script
To train the model and test its accuracy, simply run the Python script:

python SMS_Spam_Prediction.

Step 4: Predict if a New Message is Spam or Not
After training, the script will prompt you to enter a new message. Type any SMS message to check if it is spam or not, for example:


Enter a message to check if it's spam or not: "Congratulations! You've won a free iPhone. Click here to claim!"
The model will output whether the message is classified as "Spam" or "Not Spam".

Example Output

Accuracy: 0.98
              precision    recall  f1-score   support

           0       0.99      1.00      0.99       965
           1       0.98      0.91      0.94       150

    accuracy                           0.98      1115
   macro avg       0.98      0.95      0.97      1115
weighted avg       0.98      0.98      0.98      1115

Enter a message to check if it's spam or not: "Congratulations! You've won a free iPhone. Click here to claim!"
The message is: Spam
Model Performance
The performance of the model is evaluated using accuracy, precision, recall, and F1-score. The Naive Bayes classifier performs well on the SMS Spam Collection dataset with an accuracy of 98%.

![1](https://github.com/user-attachments/assets/493103c4-6ad4-4948-b6e9-f3150c24604a)
![2](https://github.com/user-attachments/assets/50ffdcc6-6e67-4608-a0cf-47842ee900e2)
![3](https://github.com/user-attachments/assets/0cd9ee95-5c11-492d-bfce-72c5c7f37773)
![4](https://github.com/user-attachments/assets/1083fbc9-6848-4032-90e4-b2519ee0377e)


License
This project is licensed under the MIT License. See the LICENSE file for details.

References
Dataset: Almeida, T. & Hidalgo, J. (2011). SMS Spam Collection [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5CC84.
Naive Bayes Algorithm: More details about Naive Bayes can be found in the scikit-learn documentation.

Files in the repository:
sms_spam_detection.py: The Python script containing the machine learning code.
requirements.txt: Lists all the necessary dependencies.

README.md: This README file with instructions and information about the project.
LICENSE: A license file (optional, but recommended).
