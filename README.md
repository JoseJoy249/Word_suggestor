Word suggestion is the task to predicting next likely words, given some words. Applications of
this include sentence completion, text suggestion in messaging services, code completion in
Integrated Development Environments (IDE) etc. In this project, an n-gram mixture model was
created to accomplish this task.
An n-gram is a contiguous sequence of n items from a sequence of text or speech. An n-gram
model is a type of probabilistic language model for predicting the next item in such a sequence in
the form of a Markov model, with n-1 states. Benefits of n-gram models include simplicity and
scalability – with larger n, a model can store more context with a well-understood space–time
tradeoff, enabling small experiments to scale up efficiently.
The model makes use of a combination of unigrams (single words), bigrams (2 word combinations)
and trigrams (3 word combinations) to predict the next likely word to come after a sequence of
words. This mixture model makes weighted predictions based on three individual models
(unigrams, bigrams and trigrams respectively) to suggest next likely word.
For this project, I collected text data from the following open sources
1. UCI Machine Learning Repository (Sentence Classification Data Set)
2. Reuters-21578 Text Categorization Collection
3. Ana Cardoso Cachopo's Homepage - http://ana.cachopo.org/
4. Peter norvig's website - http://norvig.com/
5. Brown corpus - http://www.sls.hawaii.edu/bley-vroman/brown_corpus.html
Collating from these sources resulted in a text corpus of about eleven million words. The text files
obtained were parsed in python to convert all words to lower case, remove punctuations etc. Each
individual word, two word sequences (bigrams) and three word sequences (trigrams) were stored
in three different lists. Three separate dictionaries were also created to store the counts of each
unique n-gram.
Total Number of words parsed = 10,950,156
