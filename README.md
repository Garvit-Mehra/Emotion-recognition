# 🎧 Emotion Recognition from Audio Using CNNs

This repository implements a complete pipeline for recognizing emotions in speech audio using Mel-Frequency Cepstral Coefficients (MFCCs) and a Convolutional Neural Network (CNN).

---

## 📂 Project Overview

This project is divided into two key stages:

1. **Feature Extraction** – Converts raw audio files into MFCC feature representations.
2. **Model Training & Evaluation** – Trains a CNN model to classify the emotion expressed in the audio.

---

## 🚀 Setup Instructions

Follow these steps to get started:

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/emotion-recognition-cnn.git
cd emotion-recognition-cnn
```
2. Install Required Packages

All dependencies are listed in requirements.txt. Install them with:
```bash
pip install -r requirements.txt
```
3. Download the Dataset

Download the RAVDESS Dataset (Ryerson Audio-Visual Database of Emotional Speech and Song).
	•	Extract the downloaded ZIP.
	•	Place all .wav files into a folder (e.g., ./audio_data/).

⸻

🔧 Running the Code

Step 1: Extract MFCC Features

Run extraction.ipynb:
	•	This notebook processes all .wav files and extracts MFCC features.
	•	It generates two files:
	•	X_mfcc.npy — Feature array (MFCCs)
	•	y_labels.npy — Corresponding emotion labels

Step 2: Train the CNN Model

Run model.ipynb:
	•	Loads the precomputed .npy files.
	•	Builds and trains a CNN using Keras.
	•	Evaluates the model and visualizes performance using accuracy curves, confusion matrix, and classification report.

⸻

🗂️ File Structure
