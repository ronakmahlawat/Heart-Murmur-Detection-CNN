#  Heart Murmur Detection using Deep Learning (CNN)

An end-to-end Deep Learning project for automatic **Heart Murmur Detection** from **Phonocardiogram (PCG) heart sound recordings** using **Convolutional Neural Networks (CNN)**.

The project preprocesses raw heart sound recordings, converts them into spectrogram-based representations, trains a CNN model, and classifies recordings as **Murmur Present** or **Absent**.

---

## 📌 Project Overview

Heart murmurs are abnormal heart sounds caused by turbulent blood flow. Early detection can help diagnose serious cardiovascular diseases.

This project performs:

- Audio preprocessing
- Noise reduction
- Spectrogram generation
- CNN-based classification
- Patient-level prediction
- Model evaluation

---

## 🚀 Features

- Heart Sound Classification
- CNN Deep Learning Model
- STFT Spectrogram Generation
- Mel Spectrogram Features
- Butterworth Bandpass Filtering
- Dataset Balancing
- Patient-Level Prediction
- Performance Visualization

---

# 📂 Project Structure

```
Heart-Murmur-Detection-CNN/
│
├── dataset/
│   ├── README.md
│   └── dataset_link.md
│
├── images/
│   ├── dataset_distribution.png
│   ├── waveform_spectrogram_examples.png
│   ├── preprocessing_comparison.png
│   ├── training_curves.png
│   ├── window_confusion_matrix.png
│   ├── patient_confusion_matrix.png
│   └── final_test_confusion_matrix.png
│
├── notebooks/
│   └── CNN.ipynb
│
├── report/
│   └── HeartMurmur_ProjectReport.pdf
│
├── src/
│
├── requirements.txt
├── LICENSE
└── README.md
```

---

# 🧠 Deep Learning Pipeline

```
Raw Heart Sound
        │
        ▼
Bandpass Filtering
        │
        ▼
Normalization
        │
        ▼
Feature Extraction
(STFT + Mel Spectrogram)
        │
        ▼
CNN Model
        │
        ▼
Heart Murmur Prediction
```

---

# 📊 Dataset Distribution

The dataset contains recordings from both murmur-positive and murmur-negative patients.

![Dataset Distribution](images/dataset_distribution.png)

---

# 🔊 Signal Visualization

Example PCG recordings along with their generated STFT Spectrogram and Mel Spectrogram.

![Waveform Examples](images/waveform_spectrogram_examples.png)

---

# ⚙️ Audio Preprocessing

The preprocessing stage improves signal quality before feature extraction.

Steps performed:

- Butterworth Bandpass Filter
- Noise Removal
- Signal Normalization
- PSD Analysis

![Preprocessing](images/preprocessing_comparison.png)

---

# 🧠 CNN Architecture

Input

↓

Convolution Layer

↓

ReLU Activation

↓

Max Pooling

↓

Convolution Layer

↓

Batch Normalization

↓

Flatten

↓

Dense Layer

↓

Dropout

↓

Output Layer (Softmax)

---

# 📈 Model Training

Training and validation performance over epochs.

- Training Loss decreases steadily.
- Validation Accuracy stabilizes around **88%**.

![Training Curves](images/training_curves.png)

---

# 📉 Window-Level Performance

Evaluation performed on individual audio windows.

![Window Confusion Matrix](images/window_confusion_matrix.png)

---

# 👨‍⚕️ Patient-Level Performance

Predictions are aggregated across windows to obtain final patient diagnosis.

Patient Accuracy:

**86.6%**

![Patient Confusion Matrix](images/patient_confusion_matrix.png)

---

# 🏆 Final Test Performance

Final evaluation on unseen patients.

| Metric | Value |
|---------|--------|
| Accuracy | **87.7%** |
| CNN | ✔ |
| Binary Classification | ✔ |
| Patient-Level Prediction | ✔ |

![Final Confusion Matrix](images/final_test_confusion_matrix.png)

---

# 🛠️ Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Librosa
- SciPy
- Matplotlib
- Scikit-Learn
- Jupyter Notebook

---

# 📦 Installation

Clone the repository

```bash
git clone https://github.com/ronakmahlawat/Heart-Murmur-Detection-CNN.git
```

Move into project

```bash
cd Heart-Murmur-Detection-CNN
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch notebook

```bash
jupyter notebook
```

---

# ▶️ Usage

Open

```
notebooks/CNN.ipynb
```

Run all cells sequentially.

The notebook performs:

- Dataset loading
- Audio preprocessing
- Spectrogram generation
- CNN training
- Model evaluation
- Prediction visualization

---

# 📚 Future Improvements

- Vision Transformer (ViT)
- EfficientNet
- Mobile Deployment
- Real-Time Heart Sound Classification
- Explainable AI (Grad-CAM)
- Multi-Class Murmur Classification

---

# 👨‍💻 Authors

**Ronak Mahlawat**

Electronics & Communication Engineering (Minor in Computer Science)

---

# 📄 License

This project is licensed under the MIT License.

---

⭐ If you found this project useful, consider giving it a star.
