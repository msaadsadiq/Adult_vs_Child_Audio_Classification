# Adult vs Child Speech Classification with Deep Learning

## Abstract

In this project we adapt the model from [Choi et al.](https://github.com/keunwoochoi/music-auto_tagging-keras) to train a custom music genre classification system with our own genres and data. We then use the music genre classification as a speech classification model. The model takes as an input the spectogram of audio samples from Adults and Children. It analyzes the image using a Convolutional Neural Network (CNN) plus a Recurrent Neural Network (RNN). The output of the system isthe predicted class of the audio sample either Adult or Child. 

## Code 

In this repository we provide the scripts to fine-tune the pre-trained model to re-use a music genre prediction algorithm to be used as an Adult-Child classifier. Since we have millions of annotated songs to train on, the model generally performs better on models train only on adult and child voices. Moreover, data for clean and annotated adult / child voices is very hard to get. 

### Prerequisites

We have used Keras running over Theano to perform the experiments. Was done previous to Keras 2.0, not sure if it will work with the new version. It should work on CPU and GPU. 
- Have [pip](https://pip.pypa.io/en/stable/installing/) 
- Suggested install: [virtualenv](https://virtualenv.pypa.io/en/stable/)

Python packages necessary specified in *requirements.txt* run:
```
 # Create environment
 virtualenv env_song
 # Activate environment
 source env_song/bin/activate
 # Install dependencies
 pip install -r requirements.txt
 
```

### Example Code

Fill the folder music with songs. Fill the example list with the song names. 
```
 python quick_test.py
 
```


