# Flipkart Product category Classification(NLP)
## Task: To predict product category using product description
The Task is Requirements are NLP(Natural Language Processing) and classification models.
I have done this task in the Jupyter Notebook on Google colab as it provides good computations power(Higher RAM,Higher Space,GPU).

## Approach for this Model
### Importing Libraries
![image](https://user-images.githubusercontent.com/49396916/114276732-951c1a80-9a45-11eb-8978-89032c0dcc79.png)
All important libraries are imported which are going to use in the model building(sklearn.naive_bayes,sklearn.linear_model),visualization(seaborn,matplotlib),text cleaning(nltk,restem.porter,stopwords),data preprocessing(labelencoder,standardscaler).
### Importing Dataset
![image](https://user-images.githubusercontent.com/49396916/114276822-f9d77500-9a45-11eb-8e98-95e4c5cb3a9d.png)
### Data Cleaning
![image](https://user-images.githubusercontent.com/49396916/114276859-24c1c900-9a46-11eb-817b-1e03efc55489.png)
1. I have cleaned the data by rmoving symbols,numbers,stopwords and converting all to  lower case and stemmed the data by porter stemmer.
2. I try to use Tfidf vectorizer but the model crashes durinf model fitting so that's why i leave that.
### Data Visualization
![image](https://user-images.githubusercontent.com/49396916/114277025-04463e80-9a47-11eb-9e99-93150051c6bc.png)
I have also tried to use other plots but due to a lot of classes it seems hard to plot figures I used matplotlib, seaborn but only distplot works well.
### Data Labelling/preprocessing
![image](https://user-images.githubusercontent.com/49396916/114277181-c1d13180-9a47-11eb-8baa-2bcb79072031.png)
labelencoder Normalize the data and convert non-numerical data to numerical data
### Model Building and Model Validation
![image](https://user-images.githubusercontent.com/49396916/114277297-3c01b600-9a48-11eb-9897-bbeaf74914ad.png)
Till Now the data is cleaned , visualized and preprocessed and in this phase model building will be done.Here I used Multinomial Naive Bayes modelfor classification and also verified its performance.
### Overfitting Checking and Logistic Regression
![image](https://user-images.githubusercontent.com/49396916/114277406-af0b2c80-9a48-11eb-9cc5-acc1c96f1ba7.png)
A model shows overfitting  when there is a big difference between accuracies on model prediction on test data and trained data but this is not the case here so we can say the model do not overfits
### Logistic Regression(overfitting check)
![image](https://user-images.githubusercontent.com/49396916/114277537-38226380-9a49-11eb-97dd-de3e275e328f.png)
There is also no overfitting in logistic regression model and also it has limitations, no. of iterations are limited(we can alter that but it will also increase the runtime).
I also tried to train different model but due to large amount of data the model become complex which results  crashing of RAM.
