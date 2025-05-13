# 🧠 English to French Neural Machine Translation

This project implements a **Sequence-to-Sequence (Seq2Seq)** model for translating **English sentences into French** using deep learning. It leverages **FastText word embeddings** to improve performance on rare and out-of-vocabulary words.

---

## 📌 Project Highlights

- 🔤 **English → French translation** using LSTM-based encoder-decoder architecture.
- ⚡ **FastText embeddings** integrated for better semantic understanding.
- 🧹 Preprocessing includes tokenization, padding, and vocabulary analysis.
- 📉 Training includes early stopping and learning rate scheduling.
- 📊 Evaluation with sample predictions and loss curves.
- 🔍 Custom data exploration: word clouds, frequency stats, and sentence length analysis.

---

## 📁 Dataset

The dataset used is a CSV file (`eng-french.csv`) containing two columns:
- `English words/sentences`
- `French words/sentences`

> Ensure this file is stored in a `data/` directory relative to the notebook.

---

## 🏗️ Model Architecture

- **Embedding Layer** initialized with FastText word vectors.
- **Encoder**: LSTM that processes input English sentences.
- **RepeatVector**: Prepares output shape for decoder.
- **Decoder**: Another LSTM layer followed by a TimeDistributed Dense layer with softmax.
- **Loss Function**: Sparse Categorical Crossentropy.
- **Optimizer**: Adam.

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/english-french-translation.git
   cd english-french-translation
   ```
2. Download FastText English vectors:
    [FastText](https://fasttext.cc/docs/en/english-vectors.html)

## 🧪 Sample Result

| Input (English)       | Predicted Translation (French) |
|------------------------|-------------------------------|
| How are you?           | Comment ça va ?               |
| I am hungry.           | J'ai faim.                    |
| What is your name?     | Comment tu t'appelles ?       |

---

## 🧰 Tools & Technologies

- Python 🐍  
- TensorFlow / Keras 🔧  
- FastText (word embeddings)  
- Pandas, Seaborn, Matplotlib 📊  
- Jupyter Notebook 📓  

---

## ✨ Future Improvements

- ✅ Add attention mechanism   
- ✅ Use beam search for better inference quality.  
- ✅ Support multi-language translation.  
- ✅ Deploy using a simple Flask or Streamlit UI.  

---

## 🙌 Acknowledgements

- FastText word vectors by [Facebook Research](https://fasttext.cc/)  
- Inspired by TensorFlow and Keras Seq2Seq tutorials  

