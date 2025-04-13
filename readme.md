# Audio Classification 🎤

Audio Classification is a machine learning task that involves identifying and tagging audio signals into different classes or categories. The goal of audio classification is to enable machines to automatically recognize and distinguish between different types of audio, such as music, speech, and environmental sounds.

<img src="pics\audio-preprocessing-feature-extraction-machine-learning-based-classification.png" width="600">

This deep learning project belongs to voice classification of 22 people. This project is built with the aid of [pydub](https://github.com/jiaaro/pydub). Finally, a telegram bot has been created that receives speech and predicts the name of the speaker.


## How to install
Run this command:
```
pip install -r requirements.txt
```

## How to run
+ Collect the sounds of as many people as you want in raw_data folder.
+ Perform post-processing on the data using `make_dataset.ipynb`.
+ Run this command to train model on your own dataset:

```
jupyter nbconvert --to script train.ipynb
```

+ Run this command to run inference:

```
jupyter nbconvert --to script inference.ipynb
```

+ Run this command to run telegram bot:

```
jupyter nbconvert --to script pydio_classifier_bot.ipynb
```

## Results

<img src="pics\output.png" width="500">

Output
| Accuracy | Categorical Ccrossentropy Loss |
| --------------- | --------------- |
| 0.88 | 0.43 |
