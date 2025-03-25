# Gendered Abuse Detection in Indic Languages - ULI Dataset

## Overview
This repository contains implementations of two baseline models for detecting gendered abuse in Indic languages using the ULI dataset:
- **CNN + BiLSTM Model**
- **Simple RNN Model**

The dataset includes multiple Indic languages, with separate notebooks for each language. The models are trained to classify text based on the presence of gendered abuse.

## Dataset
The dataset consists of labeled textual data in multiple Indic languages, where each instance is annotated for gendered abuse.

### Languages Covered:
- Hindi
- English
- Tamil

## Model Details
### CNN + BiLSTM
This model combines Convolutional Neural Networks (CNN) for feature extraction with a Bidirectional Long Short-Term Memory (BiLSTM) network for sequence modeling.

### Simple RNN
A basic Recurrent Neural Network (RNN) that captures sequential patterns in the text.

## Dependencies
Ensure the following packages are installed before running the notebooks:
```bash
pip install tensorflow pandas numpy seaborn scikit-learn scikit-multilearn
fastext embeddings for tamil and Hindi from -> https://fasttext.cc/docs/en/crawl-vectors.html
Glove embeddings for english -> https://nlp.stanford.edu/projects/glove/
```

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/sujalsoni26/Gendered-Abuse-Detection-in-Indic-Languages
   In mid-evaluation branch, there are jupyter files for each languages and each model which can be used.
   ```
2. Install dependencies as mentioned above.
3. Open and execute the relevant notebook for the desired language.

## File Structure
```
/
|-- CNN+BiLSTM_Task_3_Hindi_Final.ipynb  # CNN+BiLSTM Model for Hindi
|-- SimpleRNN_HINDI.ipynb                # Simple RNN Model for Hindi
|-- CNN+BiLSTM_Task_3_Tamil_Final.ipynb  # CNN+BiLSTM Model for Hindi
|-- SimpleRNN_Task_3_Hindi.ipynb         # Simple RNN Model for Hindi
|-- CNN+CNN_BiLSTM_English.ipynb         # CNN+BiLSTM Model for Hindi
|-- SimpleRNN_English.ipynb              # Simple RNN Model for Hindi
|-- models/                              # Saved model weights 
|-- Outputs/                              # outputs for each model and task 


```

## Citation
we are using ULI dataset for this task
```

