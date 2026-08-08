# 🧠 Deep Learning Projects Repository

Welcome to the **Deep Learning Projects** repository! This repository serves as a practical portfolio and learning hub featuring end-to-end implementations of foundational Deep Learning architectures: **Artificial Neural Networks (ANN)**, **Convolutional Neural Networks (CNN)**, and **Recurrent Neural Networks (RNN)**.

---

## 📌 Table of Contents
- [Architectures Explained](#-architectures-explained)
  - [1. Artificial Neural Networks (ANN)](#1-artificial-neural-networks-ann)
  - [2. Convolutional Neural Networks (CNN)](#2-convolutional-neural-networks-cnn)
  - [3. Recurrent Neural Networks (RNN / LSTM / GRU)](#3-recurrent-neural-networks-rnn--lstm--gru)
- [Summary Comparison](#-summary-comparison)
  
---

## 🌌 Architectures Explained

### 1. Artificial Neural Networks (ANN)
* **Best Used For:** Tabular / Structured Data (CSV files, SQL tables, numerical records)
* **Core Concept:** Fully Connected (Dense) Layers

#### Overview
An Artificial Neural Network (or Multi-Layer Perceptron) is the foundation of deep learning. It consists of an **Input Layer**, one or more **Hidden Layers**, and an **Output Layer**. Every neuron in a given layer connects to every neuron in the subsequent layer via weighted connections.

* **Key Mechanisms:** Forward propagation (calculating predictions) and Backpropagation using Gradient Descent (updating weights to minimize loss).
* **Strengths:** Excellent general-purpose function approximators for structured, non-sequential data.
* **Limitations:** Treats each feature independently without spatial or temporal context.

---

### 2. Convolutional Neural Networks (CNN)
* **Best Used For:** Spatial / Visual Data (Images, Video frames, Spectrograms)
* **Core Concept:** Local Feature Extraction via Convolutions & Pooling

#### Overview
CNNs are engineered to process multidimensional spatial data. Instead of connecting every pixel to every neuron, a CNN slides small filter kernels over the input to detect local features like edges, textures, shapes, and complex patterns.

* **Key Layers:**
  * **Convolutional Layer:** Extracts spatial feature maps.
  * **Pooling Layer (e.g., Max Pooling):** Downsamples feature maps to reduce spatial dimensions and computation.
  * **Dense (Fully Connected) Layer:** Maps extracted features to final output classes.
* **Strengths:** Parameter efficient and **Translation Invariant** (can recognize objects regardless of where they appear in an image).

---

### 3. Recurrent Neural Networks (RNN / LSTM / GRU)
* **Best Used For:** Sequential / Time-Series Data (Text, Speech, Audio, Financial Trends)
* **Core Concept:** Internal Memory / Feedback Loops

#### Overview
Unlike ANNs and CNNs where inputs are assumed to be independent, RNNs process sequential data **one step at a time** while retaining an internal **hidden state (memory)**. This allows the network to remember context from previous time steps.

* **Variants (LSTM & GRU):** Standard RNNs struggle with long sequences due to the *vanishing gradient problem*. Advanced architectures like **Long Short-Term Memory (LSTM)** and **Gated Recurrent Units (GRU)** use gating mechanisms to store and forget information over longer time horizons.
* **Strengths:** Captures temporal order, historical dependencies, and handles variable-length sequence inputs.

---

## 📊 Summary Comparison

| Metric / Aspect | ANN (Dense Network) | CNN (Convolutional) | RNN / LSTM (Recurrent) |
| :--- | :--- | :--- | :--- |
| **Primary Data Type** | Structured / Tabular | Visual / Spatial (2D/3D) | Sequential / Time-Series |
| **Input Shape** | 1D Feature Vector | 2D/3D Tensor (H × W × C) | 3D Tensor (Batch × Steps × Features) |
| **Core Layers** | `Dense` / `Linear` | `Conv2D`, `MaxPool2D` | `SimpleRNN`, `LSTM`, `GRU` |
| **Primary Use Case** | Classification / Regression on tabular data | Image recognition, Object detection | Text processing, Stock/Weather forecasting |

---
