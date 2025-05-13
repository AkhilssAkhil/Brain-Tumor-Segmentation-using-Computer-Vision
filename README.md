
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

yaml
Copy
Edit

---

## 🧪 Requirements

Install dependencies using:

```bash
pip install -r requirements.txt


▶️ How to Run the Project
🔧 Train the Model
Place your MRI images in images/ and corresponding masks in masks/.

Run:

bash
Copy
Edit
python train.py
This will train a U-Net model and save:

checkpoints/unet_best.h5

unet_final.h5

🌐 Launch the Streamlit Web App
Once training is complete or if you already have a model (.h5 format):

bash
Copy
Edit
streamlit run app.py
Features:

Upload your own MRI image

Optionally upload a .h5 model

Visualize original image, probability map, segmented mask, and overlay

Download the final mask output

📊 Evaluation
To evaluate the trained model on a test dataset:

bash
Copy
Edit
python evaluate.py
Make sure your test images are in:

data/test/images/

data/test/masks/

🧠 Typical Usage
Doctors or radiologists upload an MRI scan.

The system segments the tumor in real-time.

Results are visualized and downloadable.

Can be integrated into telemedicine platforms.

🧬 Dataset
Brain Tumor MRI Dataset (Google Drive)

MRI Images (Grayscale)

Masks (Binary: 0 = healthy, 255 = tumor)

Input size normalized to 256x256

📈 Metrics Used
Dice Coefficient

Intersection over Union (IoU)

Precision & Recall

Inference Time

📦 Project Deliverables
Trained U-Net model

Streamlit Web App

Evaluation Scripts

Preprocessing Modules

Documentation & Results

📚 Tech Stack
Python

OpenCV

TensorFlow / Keras

Streamlit

NumPy, scikit-learn

🔒 License
This project is for educational and research purposes only. Not for clinical use without medical approval.

yaml
Copy
Edit

---

### ✅ `requirements.txt`

```txt
numpy
opencv-python
streamlit
tensorflow>=2.10
scikit-learn
