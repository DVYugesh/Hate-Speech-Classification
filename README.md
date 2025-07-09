# Hate Buster
Hate Buster is a Deep learning model which classifies portuguese sentences into hate and non hate.
This idea was taken from the research paper{}.
## Introduction 
We all know the impact level of social media in the society. Due to the privacy of users it
also increase aggressive behaviours of users in various contexts. Detecting and address-
ing hate speech is crucial for creating a safe online environment. This paper talks about
various researches of analysing speech(hate / not hate) in different languages. There was
also a Multi lingual dataset which tries to compares the nuances between the obscene
words in the languages .The dataset that was created in this paper is called **Tupy-E** dataset which have for each
tweets/comments whether it is hate and if it is hate speech then further classifies into **11** categories of hate.

The goal was to implement the model as done in the research paper and 
then to improve the accuracy of the model.
* So to implement as such in paper we fine tuned Bertimbau(famous model for portuguese language) both base and large for  tupy-e dataset.
We got the accuracy same as in the paper{Enter the values}.
* In the first attempt we tried using an LSTM layer top on pretrained Bert which decrease the accuracy to (85%).
* Then we tried using CNN's over BERT which gave very good result and increased the accuracy to (95%).
* Trying to improve the model ,explored various techniques by using gradualunfreezing technique,Attentions Masking.
** Unfreezing technique is that we unfreeze the parameters of each layer of Bertimbau which means there parameters will also be trained but gradually with each epoch.
** Attention Masking : **Yugesh should tell me about this**.
** Instead of BERT tried using **Roberta** which is model i think trainged on 3 languages**AS FAR AS REMEMBER**.
**ALL OF OUR CODE WAS WRITTEN BY GPT DONT ASK ANY QUESTIONS BASED ON THAT**.
