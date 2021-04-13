# Investigation-on-various-Techniques-of-Sentence-Embedding-using-Question-Answering-System

**PURPOSE: **

<p align="justify">Automatic question-answering is a classical problem in natural language processing, which aims at designing systems that can automatically answer a question, in the same way as human does. The need to query information content available in various formats including structured and unstructured data has become increasingly important. Thus, Question Answering Systems (QAS) are essential to satisfy this need. QAS aim at satisfying users who are looking to answer a specific question in natural language.Moreover, it is a representative of open domain QA systems, where the answer selection process leans on syntactic and semantic similarities between the question and the answering text snippets. Such approach is specifically oriented to languages with fine grained syntactic and morphologic features that help to guide the correct QA match. Furthermore, word and sentence embedding have become an essential part of any Deep-Learning-based natural language processing systems as they encode words and sentences in fixed-length dense vectors to drastically improve the processing of textual data.
The project will concentrate on incorporating the sentence embedding with its various techniques like Infersent and BERT in the construction of Question Answering systems.Also, the latest results of the QAS system with new sentence embedding criteria implementation and describe the design and implementation of the whole QA process and provide a new evaluation of the QAS system with the sentence embedding techniques measured with an expanded version of Simple Question-Answering Database, or SQuAD.

**Download the SQuAD Dataset** from here https://www.kaggle.com/stanfordu/stanford-question-answering-dataset

**BERT MODEL:**
The BERT model is fine-tuned by first initialising it with the pre-trained parameters and then fine-tuning all of the parameters using labelled data from the downstream tasks. Even though they are all started with the same pre-trained parameters, each downstream task has its own fine-tuned model. 
Pre-training is costly (4 days on 4 to 16 Cloud TPUs), but it is a once-off procedure. A number of pre-trained models have been released by BERT. Fine-tuning is a inexpensive process. On a single Cloud TPU, or a few hours on a GPU, all of the results in the paper can be replicated in under an hour. SQuAD, for example, can be trained on a single Cloud TPU in about 30 minutes and achieve a Dev F1 score of 91.0 %.
Moreover, the BERT model is also used for **WikiQA dataset** which is described in the above folder where, the instructions are followed to run the code.

**INFERSENT MODEL:**
Facebook's latest sentence embedding model is called InferSent (as of early 2019). It's by far the most successful and only supervised sentence embedding technique I've seen so far. It refutes the notion that supervised learning produces lower-quality embeddings.

The Stanford Natural Language Inference Corpus, which consists of 570K sentence pairs that are either related neutrally, contradict each other, or imply each other, is used to train the InferSent model. The labels are labelled appropriately.

The benefit of learning the relationships between the pairs is that it allows to gain context knowledge. InferSent assigns weights to each word embedding based on the learned context of the sentences (Glove embeddings were used here, but any other embeddings could be used).

Glove Embedding
To generate word embeddings, Glove uses a count-based method. It tracks the frequency of the words used in the corpus using a co-occurrence matrix of words against content and assigns a numeric representation to each word based on the frequency.


**Download the Infersent by these command**

curl -Lo examples/infersent1.pkl https://dl.fbaipublicfiles.com/senteval/infersent/infersent1.pkl
curl -Lo examples/infersent2.pkl https://dl.fbaipublicfiles.com/senteval/infersent/infersent2.pkl

Download the Glove Embedding File from here https://www.kaggle.com/takuok/glove840b300dtxt</p>
