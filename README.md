## Speech Emotion Recognition (SER)

## Executive Summary:

As emotions play a vital role in communication, the detection and analysis of the same is of vital mental importance in today’s digital world of remote communication.  Human emotions can be detected and analysed in numerous way such as audio properties, facial expression, body gesture.

One application for audio speech emotion recognition on business enterprises would be on call centres.

For an application like call centres, the business objective is to primarily to forecast individuals' behavioral tendencies, towards achieving the ultimate analysis of the true behavioural and characteristics of the caller.

This increases customer retention, improving call handling efficiency, in-depth understanding of the emotions of a caller will lower average call length and increase efficiency along with customer experience, the ability to differentiate between happy, neutral, uncertain, disappointed or displeased moods, eliminating root causes of long call, measuring customers' emotions in each call can lead to a  better understanding of their needs regarding satisfaction, to be able to react immediately to any particular situation with the analysis of the emotions of any particular customer. Business issues, competitive intelligence and marketing campaigns can also be identified.

It improves the functionality of call centres, providing targeted coaching and also gives health care support for elderly people at emergency call centers. It could be beneficial for call centers of call urgency and consequent call ranking and redistribution is based on emotion recognition in speech, giving greater priority to calls featuring emotions such as fear, anger and sadness, and less priority to calls featuring neutral speech and happiness.


With the insights gathered from using “The Ryerson Audio-Visual Database of Emotional Speech and Song” (RAVDESS) & "Crowd Sourced Emotional Multimodal Actors Dataset" (CREMA-D) datasets, the approach of using Speech Emotion Recognition (SER) system is to base on the features extracted and obtained by Mel-frequency cepstral coefficient (MFCC) spectrograms where the frequency can match more closely to what the human ear can hear.

---------------------------------

### Problem Statement:

The objective of this project is to be able to classify and predict emotions via speech recognition with a reasonable accuracy in order to improve the value of customer relationships, the quality of interactions between agents and customers as well as its functionality as an actionable business intelligence tool for call centres.

---------------------------------

### Datasets:

#### (RAVDESS) Dataset

The Ryerson Audio-Visual Database of Emotional Speech and Song (RAVDESS),and it is free to download. This dataset has 7356 files rated by 247 individuals 10 times on emotional validity, intensity, and genuineness. here the Speech files of all actors (01-24) will be used and the files are available under path ../datasets/RAVDESS. It contains 1440 files: 60 trials per actor x 24 actors = 1440. 

https://www.kaggle.com/uwrfkaggler/ravdess-emotional-speech-audio 


#### (CREMA-D) Dataset

CREMA-D is a data set of 7,442 original clips from 91 actors. These clips were from 48 male and 43 female actors between the ages of 20 and 74 coming from a variety of races and ethnicities (African America, Asian, Caucasian, Hispanic, and Unspecified). Actors spoke from a selection of 12 sentences. The sentences were presented using one of six different emotions (Anger, Disgust, Fear, Happy, Neutral, and Sad) and four different emotion levels (Low, Medium, High, and Unspecified).

https://www.kaggle.com/ejlok1/cremad

---------------------------------

### Modelling:

Applied Support Vector Machines (SVM) and Convolutional neural networks (1D-CNN & 2D-CNN)

### Summary of accuracy results:

|Model|Data Augmentation|Accuracy|
|:----|:----|:----|
|Baseline (CNN)| |21%|
|SVM| |22%|
|CNN-1D|Yes|39%|
|CNN-2D (MFCC)|Yes|52.10%|
|CNN-2D (MFCC)|No|57.40%|
|CNN-2D (Log Mel-Spectrogram)|Yes|53.40%|
|CNN-2D (Log Mel-Spectrogram)|No|54.40%|

---------------------------------

### Conclusion & Recommendations:

CNN-2D (MFCC) without data augmentation did the best at 57.4%. With this model developed, accuracy is definitely strengthened and hence predictability will be enhanced. 

Other applications can also be further developed to adapt to real time scenarios for emotive situations.

Further exploration with additional features to analyse other speech variations such as other data augmentation to be implemented
 
---------------------------------

### References:

[1] Neethu Sundarprasad, Speech Emotion Detection Using Machine Learning Techniques, San Jose State University, accessed Spring 2018 

[2] Eu Jin Lo, Speech-Emotion-Analyzer, https://github.com/ejlok1/Speech-Emotion-Analyzer, accessed 2019

[3] Muriel Kosaka, Speech Emotion Recognition Using RAVDESS Audio Dataset, https://towardsdatascience.com/speech-emotion-recognition-using-ravdess-audio-dataset-ce19d162690 , accessed October 2020

