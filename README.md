# Multi View Sentiment Corpus (MSVC)

The Multi-View Sentiment Corpus (MVSC) consists of a set of 3000 tweets 
that has been labelled by **3 annotators** considering different views related to the same post: 
* subjectivity/objectivity
*  sentiment polarity
*  implicitness/explicitness
*  presence of irony 
*  emotion

**All the labels are given for each annotator!**

Moreover, each emoji of a tweet (if present) has been labelled as positive,
negative, neutral or topic-related. This corpus has been published at EACL 2017, [click here to read the paper](https://aclanthology.org/E17-1026/). 

The MVSC corpus includes two tab-separated files:
- MVSC Tweet Corpus.csv
- MVSC Emoji Corpus.csv

The annotation has been provided for each A* annotator (A1, A2, A3).

The MVSC Tweet Corpus file is formatted as follow:
tweet_id, tweet_text, user_id, keyword, Emotion_A*, Irony_A*, Implicit-Explicit_A*, Subjectivity_A*, Tweet_Sentiment_A*

Each entry contains:
- tweet_id is the numerical ID of the tweet;
- tweet_text is the UTF-8 text of the tweet;
- user_id is the integer representation of the unique identifier for the user who emitted the post;
- keyword is the word used to retrieve the tweet, related to two popular movies: deadpool and suicidesquad;
- Emotion_A* is the emotion label: anger, anticipation,joy, trust, fear, surprise, sadness, disgust and None;
- Irony_A* is the irony label: Ironic and Not Ironic;
- Implicit-Explicit_A* is the label regarding the implicitness/explicitness: Explicit, Implicit and None;
- Subjective_A* is the label regarding the subjectivity/objectivity: Subjective and Objective;
- Tweet_Sentiment_A* is the sentiment polarity label: Positive, Negative and Neutral.


The MVSC Emoji Corpus file is formatted as follow:
tweet_id, emoji_position, Tweet_Sent_Emoji_A*

Each entry contains:
- tweet_id is the numerical ID of the tweet;
- emoji_position is the position of the emoji ordered by appereance (e.g. "2" is related to the emoji that appears as second);
- Tweet_Sentiment_A* is the label regarding the sentiment polarity and the topic-relatedness: Topic, Positive, Negative and Neutral.



Licensing

All of the data from Twitter (tweet_id, tweet_text, user_id) is covered by Twitter's Terms of Service:
https://dev.twitter.com/terms/api-terms

Authors:
* Debora Nozza, University of Milano-Bicocca (debora.nozza@disco.unimib.it)
* Elisabetta Fersini, University of Milano-Bicocca (fersini@disco.unimib.it)
* Enza Messina, University of Milano-Bicocca (messina@disco.unimib.it)


If you decide to use this dataset, please cite:

::

    inproceedings{nozza-etal-2017-multi,
    title = "A Multi-View Sentiment Corpus",
    author = "Nozza, Debora  and
      Fersini, Elisabetta  and
      Messina, Enza",
    booktitle = "Proceedings of the 15th Conference of the {E}uropean Chapter of the Association for Computational Linguistics: Volume 1, Long Papers",
    month = apr,
    year = "2017",
    address = "Valencia, Spain",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/E17-1026",
    pages = "273--280",
}
