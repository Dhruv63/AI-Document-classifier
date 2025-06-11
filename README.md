# 🧠 Aadhaar & PAN Card Image Recognition 🔍

An intelligent deep learning system for distinguishing between **Aadhaar Cards** and **PAN Cards** using image classification. Built with TensorFlow/Keras and TensorFlow.js, and trained on a custom synthetic dataset.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Made with TensorFlow](https://img.shields.io/badge/Made%20with-TensorFlow-orange.svg)
![Teachable Machine](https://img.shields.io/badge/Powered%20by-TeachableMachine-brightgreen.svg)

---

## 🧾 Project Overview

This project demonstrates the ability to classify whether an uploaded image is of an **Aadhaar card** or a **PAN card** using a Convolutional Neural Network (CNN) model. The model is trained on **synthetically generated cards** using the Python `PIL` and `Faker` libraries and then deployed for real-time use via **TensorFlow.js in the browser**.

---

## 🗃️ Dataset

- ✅ Synthetic Aadhaar Cards (generated from real-style templates)
- ✅ Synthetic PAN Cards (generated from official-style layout)
- ✅ Each sample includes randomized:
  - Names
  - Date of Births
  - Gender
  - UID/PAN Numbers
  - Signatures (PAN)

> All data is generated and anonymized using `Faker` and is **compliant with privacy regulations**.

---

## 🧠 Model Architecture

- CNN with Conv2D, ReLU, BatchNorm, and Dense layers
- Input shape: `224x224x3`
- Output: Softmax over 2 classes: `['Aadhaar Card', 'PAN Card']`
- Trained using `categorical_crossentropy` with early stopping

---

## 🚀 Live Demo

👉 Try it locally by uploading `index.html`, `model.json`, `weights.bin`, and assets to a browser or GitHub Pages!

