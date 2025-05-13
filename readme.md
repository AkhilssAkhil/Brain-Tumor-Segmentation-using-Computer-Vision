# 🧠 Brain Tumor Segmentation using Computer Vision

This project focuses on **automating the segmentation of brain tumors** from MRI images using computer vision and deep learning techniques. The system utilizes a U-Net architecture for pixel-level segmentation, combined with a Streamlit-based web interface for easy interaction.

---

## 📌 Project Highlights

- 🔍 **Automatic segmentation** of brain tumors in grayscale MRI images.
- 🧠 Uses **U-Net CNN architecture** for high-accuracy medical segmentation.
- 💻 Streamlit **web app for easy use** by doctors or researchers.
- ⚙️ Supports **custom model upload**, mask threshold adjustment, and result downloads.

---

## 📁 File Structure

├── app.py # Streamlit web interface
├── train.py # Training pipeline
├── model.py # U-Net architecture
├── data_preprocessing.py # Preprocessing for images and masks
├── evaluate.py # Evaluation using Dice coefficient
├── inference.py # Model loading and prediction
├── requirements.txt # Python dependencies