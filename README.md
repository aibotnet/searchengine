SEARCH ENGINE
=============
First crawl some Article.

To run the create index program issue the command:
python createIndex.py stopWords.dat testCollection.dat testIndex.dat

stopwords.dat is the stopwords file
testCollection.dat is the collection file
testIndex.dat is the output of the program which is the inverted index


[tf/idf]

First decompress the testCollection.dat, stopWords.dat and porterStemmer.py 
First run the create index program:
python createIndex_tfidf.py stopWords.dat testCollection.dat testIndex.dat titleIndex.dat

Then run the query index program:
python queryIndex_tfidf.py stopWords.dat testIndex.dat titleIndex.dat

stopwords.dat is the stopwords file
testCollection.dat is the collection file
testIndex.dat is the main inverted index
titleIndex.dat is the title index


Steps involved in search Engine Implementaion
1.  Tokenizing
2.  Parsing
3.  Normalization
    --capitalization
    --synonymous database(color == colour)
    --handling abbreviation(DSLR ==DigitalSLR, in == ")
4.stemming
   (play ,playing , played)

4.lemmatization
    (Lemmatisation in linguistics, is the process of grouping together the different inflected
    forms of a word so they can be analysed as a single item.In computational linguistics,
    lemmatisation is the algorithmic process of determining the lemma for a given word. Since
    the process may involve complex tasks such as understanding context and determining the part
    of speech of a word in a sentence (requiring, for example, knowledge of the grammar of a language)
    it can be a hard task to implement a lemmatiser for a new languag)

