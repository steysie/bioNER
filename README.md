# bioNER
In this repository, the files for bioNER project are stored.

## bioNER Project Description
Marina Pozhidaeva & Anastasia Nikiforova

Clinical trials often require detailed patient information, documented in clinical descriptions. Named object recognition (NER) is a fundamental natural language processing (NLP) task for extracting objects of interest (for example, disease names, drug names, and laboratory tests) from clinical notes, to further support and develop clinical and applied research.

The dataset consists of clinical notes annotated with BIO markup (beginning-inside-outside). It is available for download from Kaggle:
https://www.kaggle.com/rsnayak/hackathon-disease-extraction-saving-lives-with-ai. 

The task is to extract all the names of diseases from a given set of 20,000 paragraphs / documents in a test set, training the model on a labeled training dataset of 30,000 documents.

## Data Description

Variable Definition

**id** Unique ID for a token/word

**Doc_ID** Unique ID for a Document/Paragraph

**Sent_ID** Unique ID for a Sentence

**Word** Exact word/token

**tag** (Target) Named Entity Tag

## Models description 

The word embedding (pre-trained fasttext in the base line) will be fed to the input, and at the output we will get its tag (BIO).

One of the most common models for NER, bi-LSTM + CRF, shows the f1-score = 0.86 on the general-domain package. As part of this task, we will strive for this mark, however, since our data is limited by bio-domain, the result may vary.


## Models for download

LSTM + CRF model: https://drive.google.com/open?id=1Ij-mMy8EWQ0aphCFZpVUnmGcfHckZQb6

LSTM on pretrained embeddings: https://drive.google.com/open?id=1BwRoTNKqTkLAp3NF-wDeHX-esu-zYYLY

Filtered pretrained embeddings: https://drive.google.com/open?id=1Pm7IolxWa5juZM5RcUvN9R6SC6GKq7Ma

Sentences tagged with UDPipe in CONLLu format: https://drive.google.com/open?id=1-68F34nTyLz-SetqBMcsdqtn0n7NYjBl
