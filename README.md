# Vani: Indian Sign Language (ISL) to Text Translator

**Vani** is an AI-based application designed to bridge the communication gap between the hearing and non-hearing communities. Using computer vision and deep learning, it translates **Indian Sign Language (ISL)** gestures into **real-time text output**.

---

## Overview

While over 18 million people in India rely on sign language, very few hearing individuals are able to understand it. This barrier limits access to education, employment, and essential services.  
**Vani** was built to make communication more inclusive — by providing an accessible, real-time ISL translation tool powered by **TensorFlow** and **MediaPipe**.

---

##  Features

- **Real-time Hand Detection** using MediaPipe landmarks  
- **Gesture-to-Text Translation** via a trained CNN model  
-  **Custom Dataset Support** for scalable training  
-  **Modular Code Structure** for easy model updates and retraining  
-  **Lightweight Deployment** on Google Colab or local systems  

---
Vani/
│
├── data/ # Dataset (custom ISL gestures)
│ ├── A/ # Class folders per gesture
│ ├── B/
│ └── ...
│
├── models/ # Saved model files (.h5 or .tflite)
│
├── notebooks/
│ └── training.ipynb # Model training and evaluation notebook
│
├── src/
│ ├── main.py # Real-time gesture detection & text display
│ ├── preprocessing.py # Data preprocessing & augmentation
│ └── utils.py # Helper functions
│
├── requirements.txt # Dependencies
├── README.md # Project documentation
└── LICENSE # Open-source license


---

## 🧩 Tech Stack

- **Language:** Python  
- **Libraries:** TensorFlow, MediaPipe, OpenCV, NumPy, Pandas  
- **Environment:** Google Colab / Jupyter Notebook  
- **Model:** CNN-based image classification  

---

## ⚙️ Installation

Clone this repository:
```bash
git clone https://github.com/<your-username>/Vani.git
cd Vani


Install dependencies:

pip install -r requirements.txt


Run the application:

python src/main.py

Dataset

The dataset contains labeled ISL hand gesture images captured in varying lighting and angles.
Each gesture (A–Z, 0–9, and common words like Hello, Thank You, etc.) is stored in its respective folder.

To preprocess or use your own dataset:

python src/preprocessing.py --path <path_to_dataset>

Model Training

Open the training notebook:

notebooks/training.ipynb


Train your model:

model.fit(X_train, y_train, epochs=30, validation_split=0.2)


Save the trained model:

model.save('models/vani_model.h5')

Inspiration

The idea for Vani came while volunteering with the Sai Swayam Society for Hearing Inclusion, where I witnessed how deeply communication barriers affect the deaf community.
This project aims to use AI for social good, ensuring accessibility and inclusion for all.

Contributing

Contributions are welcome!
To contribute:

Fork this repository

Create a feature branch

Commit your changes

Open a pull request

License

This project is licensed under the MIT License — see the LICENSE
 file for details.


Acknowledgements

MediaPipe
 for hand-tracking support

TensorFlow
 for deep learning framework

Sai Swayam Society for Hearing Inclusion for inspiring this mission

Everyone working toward a more inclusive world �

