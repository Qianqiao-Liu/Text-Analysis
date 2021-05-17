# Text-Analysis
Fondamental text processing and analysis based on raw txt or prepared corpora. 

-TextClassification.ipynb runs test classification on 39451 articles on LeMonde 2003. Two Bag-of-word methods to transform words into vertors: CountVectorizer and TF-IDF are performed and compared by training with Naive Bayes for multiple classes. The former represents words in a way of One-hot vectors whereas the latter takes into account both the frequence of a term in one document as well as its occurrence in others, which lowers its final weight assigned to the vectorizer. TfidfTransformer，although realising the relation between certain entities and documents of relevant class along with its popularity in unconcerned ones, fails to catch the connection amongst words. As a result, the scores yield a conclusion that TfidfTransformer is more accurate than CountVectorizer and merely adequate for text classification. We apply, thus, a neural network using the vectors calculated by TF-IDF which improves slightly the accuracy. With regards of TF-IDF, this is almost the best score.

-Recherche_d'information.ipynb generates phrases from nltk corpora and classify texts with Machine Learning models. Both tasks contains TF-IDF transformation mentioned above. By computing propabilities of new occurrence in unigram and bigram, we update and build sentences. Then Random Forest, Naive Bayes, Logistic Regression and Linear SVC are carried out and proved to be increasingly powerful in text classification. Random Forest is remarkably weak despite it usually fulfills greatly these missions.  


-Word_embedding.ipynb explores the methology of word embedding and its implementation thanks to Collobert & Weston, GloVe, GoogleNews and FastText librabries. Calculate similarities of words and illustrate their positions and distances in vetorial space. 
  
