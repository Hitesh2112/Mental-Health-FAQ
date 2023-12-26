# Mental-Health-FAQ

## In this project I tried to implement a chatbot like FAQ for mental health questions


Used Natural Language Processing pipeline with Machine Learning algorithms for implementation of this project

Dataset used is taken from Kaggle

Steps are :
1. Importing libraries and uploading the dataset
2. Checking for null and useless variables and its correction
3. Lowercasing the text
4. Removal of Punctuations
5. Conversion of numbers to text
6. Encoding the Answers (column) using LabelEncoder
7. Tokenization
8. Lemmatization
9. Conversion of text to vectors
    1. Word2Vec (implemented using gensim library)
    2. TF-IDF
10. Modeling (here I used LinearSVC and RandomForest with both Word2Vec and TFIDF)
11. Deployment code for prediction (like a chatbot)



## Let's understand it in a little detail

Importing libraries


<img width="578" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/19794e58-7894-48fd-8baa-b94a1df036a6">


Reading the dataset


<img width="391" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/ddf70623-a51f-473e-ade3-5e33190dcbbf">


Remove Punctuations


<img width="305" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/f19968fa-59d8-452f-9763-714e79b574ed">


Removing Special letters/extra punctuations

<img width="410" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/a0bbe06a-2f7f-421e-ab46-6129ec0a560e">



Conversion of numbers to text

<img width="371" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/a471c7c8-3ea7-4026-b178-de185269a3a4">



Label Encoding

<img width="337" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/6da45c52-2005-46a9-b771-41ed5f58e93e">



Tokenization (using spacy library)


<img width="348" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/29d4f3e4-6aca-47ed-983e-d001110eea1b">



Lemmatization

<img width="410" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/64f9d11c-3204-42e3-bff9-ff8ce2dbb1fc">



Implementing word2vec using gensim library

<img width="359" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/d7abc195-0a5c-4df8-bfae-4d76c5790c06">



Vocabulary building

<img width="284" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/bd241930-9f27-42c7-ba86-1731cfac7322">



<img width="124" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/7ef45c5e-12ae-4e08-b4c8-286e9cd2f06b">




WordCloud


<img width="401" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/34058c45-c25a-42e2-aecb-66100cc47c47">



Training word2vec model on vocabulary

<img width="470" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/32ca2841-6da3-4b0c-b651-51477460e2a5">



Function for vectorising the text of dataset using the trained word2vec model

<img width="538" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/4da614f4-73b0-416a-80e0-73b2627a843a">



Spliting Training and testing dataset

<img width="646" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/ee06c54c-3d32-4f41-afb3-175070aa53fa">



LinearSVC modeling

<img width="296" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/a2d32ad7-6373-4556-aeef-cb47102c4d14">



Fitting and prediction using LinearSVC model (with word2vec embeddings)


<img width="381" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/dd6657d4-5e83-4576-b51f-a04967bafc94">



Modelling and fitting using Random Forest model (with word2vec embeddings)

<img width="265" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/1b6153df-d827-4bc5-b777-70f56c5d57ff">


using TF-IDF Vectorisation


TFIDF vectorisation

<img width="654" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/845f5410-0b70-4132-a337-8cfa578afb7a">



Modeling using LinearSVC

<img width="473" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/5daa3aad-28ff-4df1-9dd6-2d4cb2bdba2f">



Modeling using RandomForestClassifier

<img width="293" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/0fab12ab-ec3e-4b70-aeed-5077654f3a13">


Deployment as a chatbot 

for LinearSVC with TFIDF

<img width="547" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/6153c802-fd70-4a5f-8064-a01d29f9b499">



for RandomForestClassifier with Word2Vec

<img width="539" alt="image" src="https://github.com/Hitesh2112/Mental-Health-FAQ/assets/97521900/f6e334f8-4600-41bc-8e06-48774867b0f4">


#### The accuracy of LinearSVC and RandomForestClassifier with TF-IDF is 97.5 % and of RandomForestClassifier with Word2Vec is 98.75 %
