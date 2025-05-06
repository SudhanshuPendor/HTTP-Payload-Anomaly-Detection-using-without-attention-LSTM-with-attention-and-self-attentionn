# HTTP Payload Anomaly Detection

This project implements and compares three deep learning architectures for detecting anomalies in HTTP payloads:
- **LSTM without Attention**
- **LSTM with Bahdanau Attention**
- **Transformer (Self-Attention)**

The models are trained and evaluated on structured payload data to distinguish between normal and anomalous HTTP traffic. The project is built using Python, TensorFlow/Keras, and standard ML libraries.

---

## 📁 Project Structure


---

## 📊 Dataset

- **Train_data.csv** – Contains labeled HTTP payloads for training.
- **Test_data.csv** – Contains payloads for evaluating model performance.

Each row contains:
- `payload`: raw HTTP payload (string)
- `label`: 0 (normal) or 1 (anomalous)

---

## 🧠 Models

### 1. LSTM (Without Attention)
A basic sequential model using a bidirectional LSTM layer followed by dense layers for classification.

### 2. LSTM with Bahdanau Attention
Enhances the LSTM with an attention mechanism to weigh hidden states before classification.

### 3. Transformer
Applies self-attention mechanisms to capture long-range dependencies in payload sequences. Based on the original Transformer encoder architecture.

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/HTTP-Payload-Anomaly-Detection.git
cd HTTP-Payload-Anomaly-Detection

