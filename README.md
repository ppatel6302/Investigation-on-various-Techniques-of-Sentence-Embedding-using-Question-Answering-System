# Investigation-on-various-Techniques-of-Sentence-Embedding-using-Question-Answering-System

PURPOSE: 
Automatic question-answering is a classical problem in natural language processing, which aims at designing systems that can automatically answer a question, in the same way as human does. The need to query information content available in various formats including structured and unstructured data has become increasingly important. Thus, Question Answering Systems (QAS) are essential to satisfy this need. QAS aim at satisfying users who are looking to answer a specific question in natural language.Moreover, it is a representative of open domain QA systems, where the answer selection process leans on syntactic and semantic similarities between the question and the answering text snippets. Such approach is specifically oriented to languages with fine grained syntactic and morphologic features that help to guide the correct QA match. Furthermore, word and sentence embedding have become an essential part of any Deep-Learning-based natural language processing systems as they encode words and sentences in fixed-length dense vectors to drastically improve the processing of textual data.
The project will concentrate on incorporating the sentence embedding with its various techniques like Infersent and BERT in the construction of Question Answering systems.Also, the latest results of the QAS system with new sentence embedding criteria implementation and describe the design and implementation of the whole QA process and provide a new evaluation of the QAS system with the sentence embedding techniques measured with an expanded version of Simple Question-Answering Database, or SQuAD.
![image](https://user-images.githubusercontent.com/60944134/114485787-87e46480-9bda-11eb-8c9a-4a438de18fb6.png)

Download the SQuAD Dataset from here https://www.kaggle.com/stanfordu/stanford-question-answering-dataset

Download the Infersent by these command

curl -Lo examples/infersent1.pkl https://dl.fbaipublicfiles.com/senteval/infersent/infersent1.pkl
curl -Lo examples/infersent2.pkl https://dl.fbaipublicfiles.com/senteval/infersent/infersent2.pkl

Download the Glove Embedding File from here https://www.kaggle.com/takuok/glove840b300dtxt
