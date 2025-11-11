# NLP Text Processing Assignment

## Student Information
- **Name:** Ainavole Hasini Reddy
- **Student ID:** 700773828

## Overview
This repository contains Python implementations for two NLP tasks:
1. Text preprocessing with tokenization, stopword removal, lemmatization, and POS filtering
2. Named Entity Recognition (NER) and pronoun ambiguity detection

## Question 1: Text Preprocessing Pipeline

### Description
Implements a complete text preprocessing pipeline that performs:
- Tokenization
- Stopword removal
- Lemmatization (not stemming)
- POS tagging and filtering (keeps only verbs and nouns)

### Input
```
"John enjoys playing football while Mary loves reading books in the library."
```

### Output
```
Tokens: ['John', 'enjoys', 'playing', 'football', 'while', 'Mary', 'loves', 'reading', 'books', 'in', 'the', 'library', '.']

After stopwords removal: ['John', 'enjoys', 'playing', 'football', 'Mary', 'loves', 'reading', 'books', 'library', '.']

POS tags: [('John', 'NNP'), ('enjoys', 'VBZ'), ('playing', 'VBG'), ('football', 'NN'), ('Mary', 'NNP'), ('loves', 'VBZ'), ('reading', 'VBG'), ('books', 'NNS'), ('library', 'JJ'), ('.', '.')]

After lemmatization: [('John', 'NNP'), ('enjoy', 'VBZ'), ('play', 'VBG'), ('football', 'NN'), ('Mary', 'NNP'), ('love', 'VBZ'), ('read', 'VBG'), ('book', 'NNS'), ('library', 'JJ'), ('.', '.')]

Final result: ['John', 'enjoy', 'play', 'football', 'Mary', 'love', 'read', 'book']
```

## Question 2: NER and Pronoun Ambiguity Detection

### Description
Performs Named Entity Recognition and detects potential pronoun ambiguity in text.

### Input
```
"Chris met Alex at Apple headquarters in California. He told him about the new iPhone launch."
```

### Output
```
Named Entities:
  Chris - PERSON
  Alex - PERSON
  Apple - ORG
  California - GPE
  iPhone - ORG

Warning: Possible pronoun ambiguity detected!
Pronouns found: he, him
```





