# Yahoo_Answers_Text_Dataset_Classification

How to do multi-class text classification on Yahoo Answers text dataset?

1. Download the dataset from Kaggle.

2. There are 10 classes in the dataset in train.csv and test.csv:

Society & Culture

Science & Mathematics

Health

Education & Reference

Computers & Internet

Sports

Business & Finance

Entertainment & Music

Family & Relationships

Politics & Government

3. There are 4 columns in the train and test csv:

Class

Question Title

Question Content

Best Answer

4. I did preprocessing of text data for train and test csv. First, I combined "Title", "Content", "Answer" into 1 "text" column.

   Then, I did contractions processing, lowercasing, remove numbers and punctuations, tokenize, remove stopwords, and lemmatize.

   Finally, I saved the cleaned csv.

5. I dropped all the empty text row, and did TfidfVectorizer for max_features=100000, and saved the model.

6. For train dataset, I did training and validating split, and got the validation accuracy of 70 percent on Naive Bayes model.

7. For test dataset, I did training and validating split, and got the validation accuracy of 68 percent on Naive Bayes model.

8. For train and test datasets, I combined the TfidfVectorizer for train and test datasets, and got test accuracy of 70 percent on Naive Bayes model, abd 72 percent on logistic regression model.
