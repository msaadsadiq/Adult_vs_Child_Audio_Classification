# Music Genre Classification with Deep Learning

## Abstract

In this project we adapt the model from [Choi et al.](https://github.com/keunwoochoi/music-auto_tagging-keras) to train a custom music genre classification system with our own genres and data. The model takes as an input the spectogram of music frames and analyzes the image using a Convolutional Neural Network (CNN) plus a Recurrent Neural Network (RNN). The output of the system is a vector of predicted genres for the song. 

We fine-tuned their model with a small dataset (30 songs per genre) and test it on the GTZAN dataset providing a final accuracy of 80%. 

## Code 

In this repository we provide the scripts to fine-tune the pre-trained model and a quick music genre prediction algorithm using our own weights. 

Currently the genres supported are the [GTZAN dataset](http://marsyasweb.appspot.com/download/data_sets/) tags:

- Blues
- Classical
- Country
- Disco
- HipHop
- Jazz
- Metal
- Pop
- Reggae
- Rock

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


