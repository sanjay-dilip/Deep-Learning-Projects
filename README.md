# Deep-Learning-Projects

This repository showcases deep learning projects completed as part of BUAN 6382 coursework.  
Each project demonstrates the complete pipeline: data preparation, model building, training, evaluation, and insights.

---

## Projects

### 1. CIFAR-10 Image Classification (PyTorch)
- Implemented a **Feedforward Neural Network (FCNN)** and a **Convolutional Neural Network (CNN)**.
- Compared performance: CNN achieved **80.73% accuracy** vs 45.50% for the simple NN.
- Included model training curves, confusion matrix, and per-class accuracy analysis.
- [💻 Jupyter Notebook](Project1_CIFAR10_Classification/cifar10_image_classification_pytorch.ipynb)

---

### 2. Character-Level Text Generation with LSTM (NLP)
- Built an **LSTM-based RNN** for character-level text generation using *Pride and Prejudice* (Project Gutenberg dataset).
- Preprocessed 743K characters, created ~247K training sequences, and trained multiple architectures (LSTM, deep LSTM, GRU).
- Evaluated models using **Perplexity (3.77), BLEU, ROUGE, and Entropy** metrics.
- Generated coherent novel text with controllable creativity via temperature sampling.
- [💻 Jupyter Notebook](Project2_TextGeneration/character_level_text_generation_lstm.ipynb)

---

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/<sanjay-dilip>/deep-learning-projects.git
   cd deep-learning-projects
