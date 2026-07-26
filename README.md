# Advanced Network Intrusion Detection using CICIDS2017

> 🇹🇷 **Staj Projesi**
>
> Bu depo, zorunlu staj kapsamında geliştirilen ağ saldırı tespit projesinin ileri aşamasını içermektedir. Çalışmada topluluk öğrenmesi (Ensemble Learning), derin öğrenme (Deep Learning) ve boyut indirgeme (Dimensionality Reduction) yöntemleri kullanılarak CICIDS2017 veri seti üzerinde çok sınıflı saldırı tespiti gerçekleştirilmiştir.
>
> ---
>
> 🇬🇧 **Internship Project**
>
> This repository contains the advanced phase of my mandatory internship project on network intrusion detection. Ensemble learning, deep learning and dimensionality reduction techniques are evaluated on the CICIDS2017 dataset for multiclass intrusion detection.

---

# Project Overview / Proje Özeti

## 🇹🇷

Bu proje, **CICIDS2017** veri seti kullanılarak ağ saldırılarının tespit edilmesini amaçlamaktadır.

Bu depoda, daha önce hazırlanan veri ön işleme aşamasının üzerine ileri seviye makine öğrenmesi ve derin öğrenme modelleri uygulanmış, ayrıca boyut indirgeme yöntemleri karşılaştırılmıştır.

## 🇬🇧

This project focuses on multiclass network intrusion detection using the **CICIDS2017** dataset.

It extends the preprocessing stage by evaluating advanced machine learning, deep learning and dimensionality reduction techniques.

---

# Project Structure / Proje Yapısı

```
.
├── data/
│   └── README.md
│
├── notebooks/
│   ├── 01_Ensemble_Learning.ipynb
│   ├── 02_Deep_Learning_Models.ipynb
│   └── 03_PCA_Autoencoder.ipynb
│
├── requirements.txt
├── .gitignore
└── README.md
```

---

# Models Used / Kullanılan Modeller

## Ensemble Learning

- Random Forest
- XGBoost
- LightGBM
- Stacking Classifier

---

## Deep Learning

- Deep Neural Network (DNN)
- Recurrent Neural Network (RNN)
- Long Short-Term Memory (LSTM)
- Gated Recurrent Unit (GRU)
- Bidirectional LSTM (BiLSTM)
- Bidirectional GRU (BiGRU)

---

## Dimensionality Reduction

- Principal Component Analysis (PCA)
- Autoencoder

---

# Dataset / Veri Seti

## 🇹🇷

Bu projede kullanılan eğitim ve test veri dosyaları GitHub deposuna eklenmemiştir.

Bu proje, **network-intrusion-detection-ml** projesinde oluşturulan ön işlenmiş veri dosyalarını kullanmaktadır.

Notebook'lar çalıştırılmış (executed) halde paylaşılmıştır. Sonuçlar görüntülenebilir. Ancak hücreleri yeniden çalıştırmak isteyen kullanıcıların gerekli veri dosyalarını **data/** klasörüne eklemeleri gerekmektedir.

Beklenen dosyalar:

- X_train.csv
- X_test.csv
- y_train.csv
- y_test.csv

---

## 🇬🇧

The processed dataset files are not included in this repository.

This project uses the processed datasets generated in the **network-intrusion-detection-ml** repository.

The notebooks are uploaded with executed outputs, allowing users to inspect all results directly. To rerun the notebooks, place the processed dataset files into the **data/** directory.

Required files:

- X_train.csv
- X_test.csv
- y_train.csv
- y_test.csv

---

# Results / Sonuçlar

## Ensemble Learning

| Model | Accuracy |
|--------|----------|
| Random Forest | **0.9982** |
| XGBoost | **0.9983** |
| LightGBM | **0.8247** |
| Stacking | **0.9983** |

---

## Deep Learning

| Model | Accuracy |
|--------|----------|
| DNN | 0.8032 |
| RNN | 0.8944 |
| LSTM | **0.9145** |
| GRU | 0.8889 |
| BiLSTM | 0.8906 |
| BiGRU | 0.9104 |

---

## Dimensionality Reduction

| Model | Accuracy |
|--------|----------|
| Random Forest | **0.9982** |
| RF + PCA (30) | 0.9961 |
| RF + Autoencoder | 0.9905 |

---

# Requirements

- Python 3.12+
- Jupyter Notebook
- NumPy
- Pandas
- Scikit-learn
- TensorFlow
- XGBoost
- LightGBM
- Matplotlib
- OpenPyXL

Install dependencies:

```bash
pip install -r requirements.txt
```

---

# Running the Project

1. Clone the repository.

```bash
git clone <repository-url>
```

2. Place the processed dataset files inside the **data/** directory.

3. Open the notebooks in order:

- 01_Ensemble_Learning.ipynb
- 02_Deep_Learning_Models.ipynb
- 03_PCA_Autoencoder.ipynb

---

# Future Improvements

Possible future extensions include:

- Explainable AI using SHAP
- Hyperparameter optimization
- Graph Neural Networks (GNN)
- Graph Attention Networks (GAT)
- Transformer-based architectures
- Additional feature selection techniques

---

# Author

**Gülseli Ocakcı**

Computer Engineering Student

Mandatory Internship Project

2026