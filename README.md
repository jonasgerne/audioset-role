# Music Role Classification using Audioset Database
 
 Baseline by https://github.com/HareeshBahuleyan/music-genre-classification. 
 
## Requirements 
Same as the baseline code. 
Project uses Jupyther Notebook, so you probably want to install Anaconds: https://www.anaconda.com/download

### Other requirements:

tensorflow-gpu==1.3.0
Keras==2.0.8
numpy==1.12.1
pandas==0.22.0
youtube-dl==2018.2.4
scipy==0.19.0
librosa==0.5.1
tqdm==4.19.1
scipy==0.19.0
Pillow==4.1.1

## Running the model

1. Retrive audiofiles from YouTube by running ``` 1_audio_retrieval.ipynb ```.
1. Extract MEL-Spectrograms from the audio by running 
```2_plot_spectrograms.ipynb```. These are used as an input to Neural Network.
1. Train and evalute the best NN model (VGG16 on reduced dataset with transfer learning) by runing ```3.1_vgg16_reduceddata_model_transfer_learning.ipynb```.
1. Extract the so-called hand-crafted features by running ```4.2 feature_extraction and visualization.ipynb```. 
1. Train and evaluate Feature-Engineering based model by running ```4.3_feature_based_classification.ipynb```. SVM gives the best result.
1. Evaluate the ensemble of the best models by running ```5_model_ensamble.ipynb```.
