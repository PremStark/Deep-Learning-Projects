# Sentiment Analysis using RNN

A PyTorch-based Sentiment Analysis project that trains a Recurrent Neural Network (RNN) on the IMDB Movie Reviews dataset to classify textual reviews as either **Positive** or **Negative**.

---

## 📌 Features

* **Data Cleaning**: Automatically handles missing values and removes duplicate entries.


* **Text Preprocessing**:
* Normalization (lowercase conversion)


* URL, HTML tag, and punctuation removal


* Stopword filtering using `nltk`

* Word stemming via `PorterStemmer`



* **Vectorization**: Transforms preprocessed text into numerical features using **TF-IDF**.


* **Neural Network**: Implements a PyTorch Many-to-One RNN architecture with GPU acceleration.


* **Model Checkpointing**: Saves the best-performing model weights during training.



---

## 🛠️ Requirements & Installation

To run this notebook, make sure you have Python 3 and the following dependencies installed:

```bash
pip install pandas numpy torch scikit-learn nltk

```

The script will automatically download the necessary NLTK data resources (`punkt`, `punkt_tab`, and `stopwords`) during execution.

---

## 🚀 Usage

1. **Clone the Repository**:
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

```


2. **Dataset Setup**:
Ensure `IMDB_Dataset.csv` is present in the root directory. The dataset should contain two columns:


* `review`: Text of the movie review


* `sentiment`: Binary classification label (`positive` / `negative`)




3. **Run the Notebook**:
Open and execute `RNN_Sentiment.ipynb` in **Google Colab** or Jupyter Notebook. Enabling a GPU runtime (e.g., NVIDIA T4) is recommended for faster training.



---

## 📊 Model Performance

* **Preprocessing Vocabulary Size**: Top 6,000 TF-IDF features


* **Architecture**: Input Layer $\rightarrow$ Single-layer RNN (128 hidden units) $\rightarrow$ Fully Connected Layer $\rightarrow$ Sigmoid Activation


* **Accuracy**: **~86.8%** on the test dataset



---
