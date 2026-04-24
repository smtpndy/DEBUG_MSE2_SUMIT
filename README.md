# 🤖 AI Chatbot (Vanilla RNN - NumPy)

A simple conversational AI chatbot built from scratch using **NumPy + NLTK**, without using any deep learning frameworks like TensorFlow or PyTorch.

---

## 🚀 Features

* 🧠 Custom Vanilla RNN (no external ML frameworks)
* 🔤 Text preprocessing using NLTK (tokenization + lemmatization)
* 📊 Bag-of-words + one-hot encoding
* 🏷️ Intent classification system
* 💬 Interactive CLI chat interface
* 💾 Model saving & loading (no retraining needed every time)

---

## 📁 Project Structure

```
project/
│
├── chatbot.py          # Main chatbot script
├── intents.json        # Training data (intents, patterns, responses)
├── model_artifacts/    # Saved model files (auto-generated)
│   ├── rnn_weights.npz
│   ├── vocab.pkl
│   └── encoder.pkl
```

---

## ⚙️ Installation

### 1. Clone the repository

```
git clone <your-repo-link>
cd project
```

### 2. Create virtual environment (recommended)

```
python -m venv venv
venv\Scripts\activate   # Windows
```

### 3. Install dependencies

```
pip install numpy nltk scikit-learn
```

---

## ▶️ Usage

### 🔹 First Run (Training)

```
python chatbot.py --retrain
```

### 🔹 Normal Run

```
python chatbot.py
```

---

## 💬 Example

```
You   : hello
PyBot : Hello! How can I help you today?

You   : bye
PyBot : Goodbye! Have a wonderful day!
```

---

## 🧠 How It Works

1. **Preprocessing**

   * Tokenization
   * Lowercasing
   * Lemmatization

2. **Vectorization**

   * Convert words → one-hot vectors

3. **Model**

   * Vanilla RNN (tanh activation)
   * Forward + Backpropagation manually implemented

4. **Prediction**

   * Softmax output
   * Confidence threshold filtering

---

## 🐞 Bugs Fixed

* ❌ Vocabulary empty (wrong token filter)
* ❌ Zero-vector input issue
* ❌ Incorrect tanh derivative
* ❌ Softmax instability
* ❌ Confidence threshold too high

---

## ⚠️ Important Notes

* Make sure `intents.json` is in the **same directory** as `chatbot.py`
* Run the script from the correct folder
* Avoid spaces in folder names (or use quotes in terminal)

---

## 🔮 Future Improvements

* Add GUI (Tkinter / Web UI)
* Upgrade to LSTM / Transformer
* Add context-aware responses
* Deploy as API using Flask/FastAPI

---

## 👨‍💻 Author

Sumit Pandey
Computer Science Engineer | AI & Development Enthusiast

---

## ⭐ If you like this project

Give it a star ⭐ and share it!
