Toxic-Tweets-Dataset-NLP-Problem


The code performs text classification using various machine learning models for toxicity detection in tweets.
Function Description: 
The function takes a text input as a parameter and performs various preprocessing steps to clean the text.
It converts the text to lowercase to ensure uniformity in the data.
Punctuation and special characters are removed using regular expressions, leaving only alphabetic characters and spaces.
The text is tokenized, splitting it into individual words.
Stop words, common words like 'the', 'a', 'an', etc., are removed from the tokenized list.
Lemmatization is applied to each word to convert it into its base or dictionary form (e.g., 'running' to 'run', 'better' to 'good').
The cleaned tokens are joined back together to form the final preprocessed text.
The cleaned text is returned as the output of the function.
It uses the Bag of Words (BoW) and TF-IDF (Term Frequency-Inverse Document Frequency) vectorization techniques to convert the textual data into numerical features.
The data is split into training and test sets using a subset of 10,000 rows or more depending on ram size.
The code defines five different models for classification: Decision Trees, Random Forest, Naive Bayes, K-NN Classifier, and Support Vector Machine (SVM).
Each model is trained using both BoW and TF-IDF features separately.
Metrics such as precision, recall, F1-score, and ROC-AUC are calculated for each model and vectorization technique combination.
Confusion matrices and ROC curves are plotted to evaluate the performance of each model.

##Conclusion
Based on the results, the script infers TF-IDF vectorization is more suitable for models like Naive Bayes, Random-Forest, and SVM, where the importance of words in the context of the entire corpus plays a crucial role in classification.