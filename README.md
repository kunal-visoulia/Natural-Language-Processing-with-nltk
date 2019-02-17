# Natural-Language-Processing-with-nltk(natural language toolkit)
Natural-language processing (NLP) is an area of computer science and artificial intelligence concerned with the interactions between computers and human (natural) languages, in particular how to program computers to fruitfully process large amounts of natural language data.This rapidly improving area of artificial intelligence covers tasks such as speech recognition, natural-language understanding, and natural language generation.

**building a strong NLP foundation by practicing:**

- Tokenizing - Splitting sentences and words from the body of text.
- Stop words
- stemming
- Part of Speech tagging
- Chunking
- Chinking
- Named Entity Recognition

And finally 
### text classification with NLTK
using the movie reviews dataset from cornell, text classification to classify a movie review as positive or negative.

### Important terms:
1. Corpus(singular; plural is Corpora) - a Body of text. Example: A collection of medical journals.NLTK has many built in corpora.

2. Lexicon - Words and their meanings. Example: English dictionary. However, that various fields will have different lexicons.

3. Token - Each "entity" that is a part of whatever was split up based on rules. For examples, each word is a token when a sentence is "tokenized" into words. Each sentence can also be a token, if you tokenized the sentences out of a paragraph.

### DATASET PREPROCESSING STEPS
- **Removing Stop Words from Dataset**: One of the major forms of pre-processing is going to be filtering out useless data. In natural language processing, useless words (data), are referred to as stop words.

- **Stemming Words with nltk**: Stemming, which attempts to normalize sentences, is another preprocessing step that we can perform. In the english language, different variations of words and sentences often having the same meaning. Stemming is a way to account for these variations; furthermore, it will help us shorten the sentences and shorten our lookup. For example, consider the following sentence:

    I was taking a ride on my horse.<br/>
    I was riding my horse.

    These sentences mean the same thing, as noted by the same tense (-ing) in each sentence; however, that isn't intuitively     understood by the computer. **To account for all the variations of words in the english language, we can use the Porter stemmer.** So, ride,riding,rides => ride while rider=>rider and rode=>rode
- **Part of Speech Tagging with NLTK**: Part of speech tagging means *labeling words as nouns, verbs, adjectives, etc*. Even better, NLTK can handle tenses!. **PunktSentenceTokenizer**: This tokenizer is capable of unsupervised learning, so it can be trained on any body of text. It has to be trained on training text data and then it can be used to tokenize data. Then you need to tag each tokenized word with a part of speech. For list of possible tags : https://www.ling.upenn.edu/courses/Fall_2003/ling001/penn_treebank_pos.html.
- **Chunking with NLTK**: Now that each word has been tagged with a part of speech, we can move onto chunking: **grouping the words into meaningful clusters**. The main goal of chunking is to group words into "noun phrases", which is a noun with any associated verbs, adjectives, or adverbs. The part of speech tags that were generated in the previous step will be combined with regular expressions
- **Chinking with NLTK**: Sometimes there are words in the chunks that we don't won't, we can remove them using a process called chinking.
- **Named Entity Recognition with NLTK**: One of the most common forms of chunking in natural language processing is called "Named Entity Recognition." NLTK is able to identify people, places, things, locations, monetary figures, and more. There are two major options with NLTK's named entity recognition: either recognize all named entities, or recognize named entities as their respective type, like people, places, locations, etc.

