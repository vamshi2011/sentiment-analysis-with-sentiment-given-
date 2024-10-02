# sentiment-analysis-with-sentiment-given
This project is about predicting the polarity or **sentiment** of the given sentence based on the words used in the sentence. We have used the **MultinomialNB** classifier from the sklearn.naive_bayes library.

# Required Libraries
1. NLTK
2. Numpy
3. Pandas
4. Matplotlib
5. Sklearn
6. Seaborn

# Features
- **Machine Learning Model**: Built using the Multinomial Naive Bayes classifier , which is probablistic algorithm based on the bayes theorm.
- **Evaluation**: The model is evaluated by various evaluation metrics like : accuracy score , precision, recall score , confusion matrix etc.

# Dataset
The dataset is a collection of tweets collected online.It consists of 1048572 rows and 6 columns. The columns are:
- polarity of the tweet
- id of the tweet
- date of the tweet
- query
- user
- text of the tweet

There are 2 polarity of the tweet:
0 - negative 
1 - positive

# Preprocessing
- The 'id of the tweet', 'date of the tweet' , 'query', 'user' columns are removed as they are not important in knowing the sentiment of a sentence.
- As the number of rows are too large to handle , we will limit the rows to 50000 negative sentences and 50000 positive sentences. This ensures that the dataset is balanced and model can train on the dataset easily.
- The text data is converted to a vectorized format so that it can be handled by the machine learning model.

# Model Training
- The model is trained on the preprocessed dataset.
- Only the 80% of the dataset is used for training and remaining is used for testing. This is easily handled by the **train test split** class from the sklearn library.

# Input and output
The input is a sentence and based on the model training data , it classifies the sentence as positive or negative

# Instructions
1. **Clone the repo**
   ```bash
   git clone https://github.com/vamshi2011/sentiment-analysis-with-sentiment-given-.git
   ```
2. ** Launch the application**
   ```bash
   python Copy of sentiment_analysis_internzlearn.ipynb
   ```
# Open in google collab
To open the application directly in google collab , go to **"Copy of sentiment_analysis_internzlearn.ipynb"** file in github and click the **"Open in Google collab"**. There you can edit the code as per your reqirements.
