# YouTube-Spam-Filter-Using-Naive-Bayes
This repository contains a project that implements a spam filter using the Naive Bayes classification approach to classify YouTube comments as spam or non-spam.
Project Overview
Dataset
The dataset consists of comments from five YouTube videos, with the following attributes:

![Screenshot 2024-09-17 at 6 32 32 PM](https://github.com/user-attachments/assets/c2d4a18b-fd4c-4294-bd50-d49345eb27aa)

We use four datasets for training and the fifth one for testing. These datasets are:

Youtube01-Psy.csv| Youtube02-KatyPerry.csv | Youtube03-LMFAO.csv | Youtube04-Eminem.csv| Youtube05-Shakira.csv (used for testing)
# Model
The project uses the Naive Bayes classifier from the sci-kit-learn library. The text data (comments) is transformed into TF-IDF vectors to feed into the model. After training, the model is tested on the fifth dataset, and its performance is evaluated using accuracy, precision, and confusion matrix.
# Project Structure
The project contains the following main sections:
### Data Preprocessing:
The AUTHOR column is removed, and the DATE column is converted to datetime format.
The comments (CONTENT) are transformed into TF-IDF vectors using TfidfVectorizer.
# Model Training:

The Naive Bayes classifier (MultinomialNB) is trained using four datasets combined.
The number of spam and non-spam comments is recorded, and the model learns to classify based on the comment content.
# Model Testing:
The fifth dataset (Youtube05-Shakira.csv) is used for testing the trained model.
Predictions are made on the test data, and the number of correctly classified spam and non-spam comments is calculated.
## Evaluation:
The model is evaluated using metrics such as accuracy, precision, and confusion matrix.
Confusion matrix visualization is done using Seaborn heatmap.
### Results
The model achieved the following performance on the test dataset:
Accuracy: 87.3%
Precision: 83.2%
