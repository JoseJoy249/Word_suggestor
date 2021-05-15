### Objective
Word suggestion is the task of predicting next likely words, given some words. This can be utilized in use cases like  sentence completion, text suggestion in messaging services, code completion in Integrated Development Environments (IDE) etc. N-gram mixture models were used to accomplish this task.


### N-grams
An n-gram is a contiguous sequence of n items, that from a sequence of text or speech. An n-gram model is a type of probabilistic language model for predicting the next item in such a sequence, in the form of a Markov model, with n-1 states. Benefits of n-gram models include simplicity and scalability; with larger n, a model can store more context with a well-understood space–time tradeoff, enabling small experiments to scale up efficiently.

The model used in this project makes use of a combination of unigrams (single words), bigrams (2 word combinations) and trigrams (3 word combinations) to predict the next likely word to come after a sequence of words. This mixture model makes weighted predictions based on three individual models (unigrams, bigrams and trigrams respectively) to suggest next likely word.

### Dataset
For this project, I collected text data from the following open sources
1. UCI Machine Learning Repository (Sentence Classification Data Set)
2. Reuters-21578 Text Categorization Collection
3. Ana Cardoso Cachopo's Homepage - http://ana.cachopo.org/
4. Peter norvig's website - http://norvig.com/
5. Brown corpus - http://www.sls.hawaii.edu/bley-vroman/brown_corpus.html

Collating from these sources resulted in a text corpus of about eleven million words. The text files obtained were processed with python (converting all words to lower case, remove punctuations etc.). Hash maps were used to store individual word, two word sequences (bigrams) and three word sequences (trigrams) and counts.

Total Number of words parsed = 10,950,156
