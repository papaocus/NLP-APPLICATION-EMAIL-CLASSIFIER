# NLP-APPLICATION-EMAIL-CLASSIFIER

Importing necessary libraries: Streamlit, pickle, string, NLTK (Natural Language Toolkit), and PorterStemmer from NLTK.

Defining a function called transform_text() that preprocesses the input text by converting it to lowercase, tokenizing it, removing non-alphanumeric characters and stopwords, and applying stemming using PorterStemmer.

Loading the TF-IDF vectorizer and the trained model from pickle files.

Setting up the Streamlit app title as "Email/SMS Spam Classifier".

Creating a text area input where the user can enter the message to be classified.

Adding a button labeled "Predict".

When the "Predict" button is clicked, the following steps are performed:
a. The input message is preprocessed using the transform_text() function.
b. The preprocessed message is vectorized using the TF-IDF vectorizer.
c. The trained model predicts whether the message is spam or not based on the vectorized input.
d. The result of the prediction is displayed as a header in the Streamlit app.

If the predicted result is 1, it means the message is classified as spam, and "Spam hai yeh" is displayed as the header.

If the predicted result is 0, it means the message is classified as not spam, and "Spam nahi hai yeh" is displayed as the header.
