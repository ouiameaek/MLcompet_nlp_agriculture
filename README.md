# ML Competition : NLP Agricultural Keyword Spotter ( Luganda and English )

## Intro

The goal of this competition is to build a model to identify spoken agricultural keywords (in Luganda or English) in audio clips. The keywords relate to crops, diseases, fertilizers, herbicides or other general agricultural topics.
For more details checkout the [Zindi competition](https://zindi.africa/competitions/giz-nlp-agricultural-keyword-spotter)

## Overall approach

* Data augmentation (given how small the input dataset is)
* Extract features from the input audios : MFCC using [Librosa](https://librosa.org/doc/latest/index.html)
* Establish baseline models : XGboost, CNN
* Train a deep learning model from scratch : [Wavenet](https://deepmind.com/blog/article/wavenet-generative-model-raw-audio) architecture
* Train using pretrained models ( transfer learning ) : ImageNet

## Approches yet to be to explored

(with more time)

* Explore other pretrained models : ResNet, DenseNet
* Explore stacking multiple models
