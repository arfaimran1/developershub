# BERT News Classification using AG News Dataset

## Overview

This project fine-tunes a **BERT (bert-base-uncased)** model for multi-class text classification on the **AG News dataset**.
The trained model classifies news headlines into one of four categories:

* World
* Sports
* Business
* Sci/Tech

An interactive **Gradio web interface** is included for real-time predictions.

---

## Dataset

**AG News Dataset** from Hugging Face Datasets Library

* 4 News Categories
* Used subset for faster training:

  * Training Samples: 2000
  * Testing Samples: 500

---

## Technologies Used

* Python
* Hugging Face Transformers
* Hugging Face Datasets
* PyTorch
* Scikit-learn
* Gradio

---

## Model Architecture

* **Base Model:** bert-base-uncased
* **Task:** Sequence Classification
* **Output Classes:** 4

---

## Training Configuration

* Epochs: 2
* Learning Rate: 2e-5
* Batch Size: 8
* Weight Decay: 0.01
* Max Sequence Length: 128

---

## Evaluation Metrics

The model is evaluated using:

* Accuracy
* Weighted F1 Score

---

## Sample Prediction

Input:
Apple releases new AI powered iPhone

Output:
Sci/Tech

---

## Gradio Interface

The project includes a simple Gradio app for interactive testing.

Features:

* Enter any news headline
* Instantly predicts category
* Shareable web interface via Gradio

---

## How to Run

### Install Dependencies

```bash
pip install transformers datasets scikit-learn torch gradio
```

### Run Training Script

```bash
python bert_news_classifier.py
```

---

## Project Workflow

1. Load AG News Dataset
2. Tokenize Text using BERT Tokenizer
3. Fine-tune BERT Model
4. Evaluate Performance
5. Predict Custom Headlines
6. Launch Gradio Interface

---

## Future Improvements

* Train on full AG News dataset for better accuracy
* Add model saving/loading
* Deploy on Hugging Face Spaces
* Improve UI styling

---

## Author

Arfa Imran
