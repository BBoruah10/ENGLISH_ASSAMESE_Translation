# Assamese Sentence Translation using Bi-directional RNN

This project implements an English-to-Assamese sentence translator using a Bidirectional Recurrent Neural Network (RNN) with embeddings. The model's performance is evaluated using the BLEU score metric.

---

## Features
- Translates English sentences to Assamese.
- Utilizes a Bidirectional RNN with embeddings for better context understanding.
- BLEU score evaluation for accuracy measurement.

---

## Dataset
The dataset for training and testing the model is sourced from the **Corpus**. Ensure the dataset is downloaded and placed in the appropriate directory before training the model.

---

## Setup Instructions

### Prerequisites
- Python 3.7+
- Virtual Environment (optional but recommended)

### Dependencies
Install the required dependencies using pip:
```bash
pip install -r requirements.txt
```

---

## How to Use

### 1. Dataset Preparation
- Place the dataset files (English and Assamese sentence pairs) in the `data/` directory.

### 2. Training the Model
Run the training script to train the Bidirectional RNN:
```bash
python train.py
```
This will train the model using the provided dataset and save the trained weights in the `models/` directory.

### 3. Translating Sentences
Use the translation script to translate English sentences to Assamese:

The output will display the Assamese translation.

### 4. Evaluating the Model
Run the evaluation script to calculate the BLEU score:
```bash
python evaluate.py
```

---

## Directory Structure
```
project/
├── data/
│   ├── train.en # English sentences for training
│   ├── train.as # Assamese sentences for training
├── models/
│   ├── model_weights.h5 # Trained model weights
├── train.py # Training script
├── translate.py # Translation script
├── evaluate.py # Evaluation script
├── requirements.txt # Dependencies
├── README.md # Project Documentation
```

---

## Evaluation Metric
- **BLEU Score**: The model's accuracy is evaluated using the BLEU (Bilingual Evaluation Understudy) score, which compares the translated sentences with the reference translations in the dataset.

---

## Future Enhancements
- Integrating Transformer models for improved translation quality.
- Expanding the dataset to cover more diverse sentence structures.
- Adding a user-friendly web interface for real-time translations.

---

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your improvements or bug fixes.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.
