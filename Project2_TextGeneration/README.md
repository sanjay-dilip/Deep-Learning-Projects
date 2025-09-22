# Project 2: Character-Level Text Generation with LSTM

## 📌 Overview
This project implements a **character-level text generation model** using **LSTM-based Recurrent Neural Networks (RNNs)**.  
The model is trained on *Pride and Prejudice* (public domain, Project Gutenberg) and generates new text sequences in the style of Jane Austen.

The goal of this project is to:
- Explore character-level natural language processing (NLP).
- Understand the strengths and limitations of LSTMs for text generation.
- Compare different architectures (LSTM, deep LSTM, GRU) and regularization strategies.

---

## 📊 Dataset
- **Source:** [Project Gutenberg – Pride and Prejudice](https://www.gutenberg.org/files/1342/1342-0.txt)  
- **Size:** 743,375 characters (~700k).  
- **Preprocessing Steps:**
  - Lowercasing all text.
  - Removing special characters and symbols.
  - Reducing to a vocabulary of **46 unique characters** (letters, digits, punctuation, whitespace).
  - Creating **overlapping training sequences**:
    - Sequence length = 40 characters.
    - Step size = 3 characters.
    - Total training examples = ~247,000.

---

## ⚙️ Methodology
1. **Data Preparation**
   - Character-to-integer tokenization.
   - One-hot encoding of target characters.
   - Split into training (90%) and validation (10%).

2. **Model Architectures**
   - **Base Model:** Single LSTM layer (128 units).
   - **Deep LSTM:** Two stacked LSTM layers for hierarchical learning.
   - **LSTM with Dropout:** Added dropout layers for regularization.
   - **GRU Model:** Used GRU cells as a faster alternative to LSTM.

3. **Training**
   - Optimizer: Adam
   - Loss: Categorical Crossentropy
   - Epochs: 20
   - Batch size: 128 (tuned for efficiency vs. stability)

4. **Evaluation Metrics**
   - **Perplexity:** Measures predictive performance (lower is better).
   - **BLEU & ROUGE Scores:** Compare generated text with reference sequences.
   - **Diversity Metrics:**
