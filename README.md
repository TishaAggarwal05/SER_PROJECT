# 🎙️ Speech Emotion Recognition (SER)
### 🧠 Overview
The Speech Emotion Recognition (SER) system is an AI-powered project that detects and classifies human emotions based on audio input. By analyzing voice tone, pitch, and frequency features, the model can identify emotions such as happy, sad, angry, neutral, and more.
##### best accuracy achieved - accuracy: 0.9796 
### Features

- 🎧 Recognizes emotions from recorded or uploaded voice samples

- 🔊 Uses MFCCs (Mel-Frequency Cepstral Coefficients) for feature extraction

- 🤖 Built with Deep Learning for classification

- 📊 Visualizes training performance and emotion distribution

### Tech Stack

- Language: Python
- Libraries: NumPy, Pandas, Librosa, seaborn, TensorFlow / Keras
- IDE/Tools: Jupyter Notebook, VS Code
- Dataset: TESS

### Setup 

``` bash
git clone  https://github.com/TishaAggarwal05/SER_PROJECT.git                                                                  
cd SER_PROJECT
pip install -r requirements.txt
```

### Model Workflow

- Data Preprocessing – : Audio files are read from datasets like TESS and dataframe is made by labelling each audio file by python string processing
- Feature Extraction – Computed MFCCs features - 40 MFCCs are extracted per frame.
- Model Training – Train Bi-LSTM classifier on extracted features.
- Evaluation – Measure accuracy and confusion matrix

```
       precision    recall  f1-score   support

       angry       0.98      0.97      0.97        60
     disgust       1.00      0.88      0.94        60
        fear       1.00      1.00      1.00        60
       happy       0.95      0.98      0.97        60
     neutral       0.97      1.00      0.98        60
         sad       0.98      1.00      0.99        60
    surprise       0.94      0.98      0.96        60

    accuracy                           0.97       420
   macro avg       0.97      0.97      0.97       420
weighted avg       0.97      0.97      0.97       420
```
- Prediction – Classify unseen speech samples into emotion categories
