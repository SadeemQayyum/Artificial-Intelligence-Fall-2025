# Deepfake vs Real Image Detection System

This project is a deep learning based system that detects whether an image is **Real or Deepfake**. It uses EfficientNetB0, Error Level Analysis, and EXIF metadata to improve detection accuracy. A simple Gradio web interface is included for testing.

---

## Project Overview

Deepfake technology can create very realistic fake images. These images are often used for misinformation, identity misuse, and cybercrime. This system helps detect such fake images automatically using a trained CNN model. :contentReference[oaicite:0]{index=0}

---

## Features

- Real vs Fake image classification  
- EfficientNetB0 based deep learning model  
- Error Level Analysis for visual forgery detection  
- EXIF metadata extraction  
- Three phase model training  
- Live prediction with confidence score  
- User friendly Gradio web app  

---

## Dataset

The dataset is taken from Kaggle titled **Deepfake and Real Images Dataset by Manjil Karki**.  
It contains two folders:

- Fake (deepfake images)
- Real (original images)

Images include different lighting conditions, resolutions, and facial expressions. :contentReference[oaicite:1]{index=1}

A balanced **45 percent subset** of the dataset is used for training. :contentReference[oaicite:2]{index=2}

---

## Model Architecture

- EfficientNetB0 as base model  
- Global Average Pooling  
- Dense layers for classification  
- Binary output (Real or Fake)

Training is done in **three phases**:

- Phase 1: 10 epochs  
- Phase 2: 30 epochs  
- Phase 3: 20 epochs  

:contentReference[oaicite:3]{index=3}

---

## Input and Output Format

**Input:**  
Single image in JPG, JPEG, or PNG format

**Output:**  
- Prediction label (Real or Fake)  
- Confidence percentage  
- EXIF metadata  
- ELA image output  

:contentReference[oaicite:4]{index=4}

---

## Libraries Used

- TensorFlow 2.12  
- EfficientNet  
- Pillow  
- NumPy  
- Scikit learn  
- OpenCV Headless  
- Gradio  
- piexif  

:contentReference[oaicite:5]{index=5}

---

## How to Run the Project

1. Mount Google Drive  
2. Install all required libraries using pip  
3. Set dataset path  
4. Create 45 percent subset  
5. Train the model in multiple phases  
6. Evaluate using classification report  
7. Launch Gradio interface for testing  

:contentReference[oaicite:6]{index=6}

---

## Gradio Interface

Users upload an image and instantly receive:

- Real or Fake result  
- Confidence score  
- Metadata details  
- Forensic ELA image  

---

## Demo Video and Repository

- Demo Video: :contentReference[oaicite:7]{index=7}  
- GitHub Repository: :contentReference[oaicite:8]{index=8}  

---

## Project Team

- Muhammad Sadeem Choudhary  
- Muhammad Yousaf  

Faculty of Computing  
Riphah International University  
:contentReference[oaicite:9]{index=9}

---

## Expected Results

- Accuracy above 75 to 85 percent  
- Detection of blending artifacts  
- Detection of unnatural textures  
- Real time prediction interface  

:contentReference[oaicite:10]{index=10}

---

## License

This project is for educational and research purposes only.
