# Transformer-Based Stock Directional Prediction

📌 Project Overview

This project implements a Time-Series Transformer architecture to predict the directional movement of IBM stock returns. Unlike traditional models that predict absolute prices, this model focuses on Arithmetic Returns, making it more robust against market non-stationarity.

The core of the project is a custom Multi-Head Attention mechanism combined with Time2Vector embeddings, allowing the model to "attend" to critical historical events across a 128-day lookback window.

🚀 Key Features

- Transformer Encoder Architecture: Uses Self-Attention to capture non-linear dependencies in financial data.

- Time2Vector Embedding: Captures both periodic (cyclical) and non-periodic (trend) temporal patterns.

- Leakage-Free Pipeline: Implements strict chronological data splitting and incremental scaling to ensure realistic evaluation.

- Interactive Visualizations: Includes Plotly candlestick charts and training history analysis.


🛠️ Technical Stack

- Deep Learning: TensorFlow / Keras

- Data Manipulation: Pandas, NumPy

- Visualization: Matplotlib, Plotly

- Scaling: Scikit-Learn (MinMaxScaler)

🏗️ Model Architecture

The model consists of:

- Input Layer: 128-day window of OHLCV data.

- Time2Vector Layer: Learns time-based representations.

- Transformer Encoders: 3 layers of Multi-Head Attention to extract features.

- Global Average Pooling: Condenses temporal features.

Dense Layers: Fully connected layers with Dropout (0.1) for regularization.

📖 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/stock-transformer.git
2. Install dependencies:
   ```bash
   pip install tensorflow pandas numpy matplotlib plotly scikit-learn
3. Launch The Project
   ```bash
   jupyter notebook main.ipynb

⚠️ Disclaimer
This project is for educational purposes only. Trading stocks involves significant risk. This model is a research tool and should not be used as financial advice.
