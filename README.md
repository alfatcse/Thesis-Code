Here is the updated `README.md` content, formatted for direct use in your repository. I have included the citation for your published paper in a dedicated section.

-----

# One Hand Bangla Sign Language Translator

This repository contains a real-time **Bangla Sign Language (BdSL)** recognition and translation system. The project utilizes **Transfer Learning** on the **Inception v3** architecture to classify hand gestures into Bangla characters, facilitating communication between the deaf and mute community and the general public.

## 🚀 Features

  * **Real-time Sign-to-Text:** Uses a webcam and OpenCV to capture and classify gestures instantly.
  * **Text-to-Sign Translation:** A GUI that takes Bangla text input and displays the corresponding sign language images.
  * **Two-Way Communication:** Bridges the gap between sign language users and non-users.
  * **Extensive Support:** Includes recognition for Bangla vowels, consonants, and "Kar" modifiers such as া, ি, and ু.

## 🛠️ Requirements

The project is built with Python and requires the following specific versions for compatibility:

  * `tensorflow==1.2.1`
  * `opencv-python==3.2.0.8`
  * `numpy==1.13.0`
  * `matplotlib==2.0.2`
  * `Pillow` (for GUI image rendering)

Install the dependencies using:

```bash
pip install -r requirements.txt
```

## 📂 Project Overview

  * `classify_webcam.py`: The core script for real-time sign recognition using a webcam.
  * `pageChanging.py`: The Tkinter-based GUI for translating text into sign language images.
  * `train.py`: The training script used to apply transfer learning to the Inception v3 model for BdSL classification.
  * `Training_Data/`: A directory containing the dataset of gesture images.
  * `requirements.txt`: Lists all Python libraries required to run the project.

## 🚦 Getting Started

### 1\. Real-time Gesture Recognition

To launch the webcam translator:

```bash
python classify_webcam.py
```

  * **How it works:** Position your hand within the blue rectangle on the camera feed. Once a gesture is held for a few frames, the system identifies and displays the Bangla character.

### 2\. Text-to-Sign GUI

To use the visual translator:

```bash
python pageChanging.py
```

  * **Normal People to D\&M:** Enter Bangla text to see the sequence of hand signs required to communicate.
  * **D\&M to Normal People:** Launches the webcam classifier directly from the GUI.

### 3\. Training the Model

To retrain the classifier with your own dataset:

```bash
python train.py --image_dir [your_dataset_path]
```

The script analyzes subfolders in your image directory, using folder names as labels for the new classes.

## 📖 Published Paper

The methodology and results of this project are detailed in the following publication:

  * **Paper Link:** [IEEE Xplore - One Hand Bangla Sign Language Recognition](https://www.google.com/search?q=https://ieeexplore.ieee.org/abstract/document/8628158)

## 🎓 Acknowledgments

This project was developed as part of a thesis focusing on accessible technology for Bangla speakers. It utilizes the Inception v3 model architecture provided by the TensorFlow team.
