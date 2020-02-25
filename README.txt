Project Name : ImdB Sentiment Analysis

Data File:imdb-movie-reviews-dataset
aclImdb\train\pos
aclImdb\train\neg
aclImdb\test\pos
aclImdb\test\neg

File Structure: 
test.py
README.txt

Development Environment:
Text classification on IMDB review using different models and finding the accuracy of model on the test data.

Libraries used:
1) numpy : used for array operations
2) pandas : used to from a dataframe
3) nltk : used for tokenize the data and word lemmatization
4) sklearn : for importing the classifiers 
5) string : used for punctuation
6) sklearn.feature_extraction : used for vectorization
7) matplotlib : to plot charts
8) Gridsearch: used for parameter tuning of the model

Code review:
Given the data in the form of text.The data consists of two files train and test.
In each of the file there are two files(pos,neg).Read the texts form the file and label the texts with respect to
the positive and negative.Once the text data is read and labeled we form a dataframe that has columns regarding the review with 
corresponding label.

Now perform the preprocessing steps on the data.
1) Word tokenization
2) remove stopwords
3) remove non-alpha text
4) word lemmatization

Then the train data is split into train and test(valid).Since to train the model we need convert the text into vectors 
for that use vectorization process.It is a general process of turning a collection of text documents into numerical feature vectors.
This can be done using different types of vectorizers(count,tf-idf).

Train the machine learning with the train data and validate the model using the test(valid) data.Training of the model can be done
with normal text data and preprocessed text data.Now use this model on the test data and found the accuracy.
Accuracy comparsion is done on the test data considering normal data and pre-process data.

Different kinds of machine learning models is used.