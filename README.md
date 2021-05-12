## Speech Emtion Recognition (SER)

### Problem Statement

As emotions play a vital role in communication, the detection and analysis of the same is of vital mental importance in today’s digital world of remote communication. Speech is a medium through which expression of perspective and identification of one’s mental state is possible. Recognising the feelings that others are trying to convey through speech is essential. There are various parameters of the speech signal can define the feelings of a person. 

With the insights gathered from using “The Ryerson Audio-Visual Database of Emotional Speech and Song” (RAVDESS) dataset, the approach of using Speech Emotion Recognition (SER) system is to base on the features extracted and obtained by Mel-frequency cepstral coefficient (MFCC) spectrograms where the frequency can match more closely to what the human ear can hear.

With the features obtained from the extraction of the audio clips which are in a matrix format, to then model them onto traditional Machine Learning algorithms like SVM or on 1-D CNN and train the model to predict 6 classes of emotions based on the audios which are indifferent, sadness, happy, anger, surprise and fear.

