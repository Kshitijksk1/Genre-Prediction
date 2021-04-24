Requirements:
1) Jupyter Notebook/ Google Colab
2) Pandas, NumPy, sklearn

Dataset:
CMU Book Summary Dataset
This dataset contains plot summaries for 16,559 books extracted from Wikipedia, along with aligned metadata from Freebase, including book author, title, and genre.
We have used Book_id, Name, Genre, Summary and Book_Author for doing the prediction.

Details:
In this assignment we have to predict the Genre of the selected book based on the book summary. We have first done the preprocessing of the data. 
The data in the dataset is in a python dictionary format and we have to first convert the data into a Python List format. 
We now use NLTK and import the stopwords from the library and preprocess the summary field from the dataset.
In preprocessing we remove the backslash \, whitespaces ' '. We remove all special symbols except alphabets. 
Using the MultilabelBinarizer we convert the textual data into features for feature extraction. We use Tf-idf for feature extraction.
For building our model we use Logistic Regression. We can also use Poisson Regression, Decision Trees or Neural Networks also.
We use multilabel classification named OneVsRestClassifier. 
We then create the predict function to predict the Genre for the test dataset and check the accuracy of the model. 

Execution:
I have run the file on Google Colab and uploaded the dataset on my Google Drive. We can also use the dataset locally and put the local path of the dataset.

References:
 https://www.ics.uci.edu/~smyth/courses/cs175/text_data_sets.html
 http://www.cs.cmu.edu/~dbamman/booksummaries.html
 https://www.geeksforgeeks.org/detect-an-unknown-language-using-python/
 https://towardsdatascience.com/an-illustrated-guide-to-the-poisson-regression-model-50cccba15958
 https://scikit-learn.org/stable/modules/generated/sklearn.multiclass.OneVsRestClassifier.html
 https://machinelearningmastery.com/one-vs-rest-and-one-vs-one-for-multi-class-classification/
 https://scikit-learn.org/stable/modules/generated/sklearn.metrics.f1_score.html
 https://www.analyticsvidhya.com/blog/2019/04/predicting-movie-genres-nlp-multi-label-classification/
 https://stackoverflow.com/questions/26693736/nltk-and-stopwords-fail-lookuperror
 https://www.kaggle.com/ymaricar/cmu-book-summary-dataset
