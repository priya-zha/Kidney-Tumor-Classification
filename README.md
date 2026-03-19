# 🫘 Kidney Tumor Classification using Deep Learning

A deep learning-powered web application that detects kidney tumors from CT scan images. The system uses a custom CNN and a VGG transfer learning model, deployed via a Streamlit interface where users can upload CT scan images and receive an instant tumor/normal prediction.

---

## 📌 Description

Kidney cancer (renal cell carcinoma) is a top-10 cancer globally. Early detection through CT scans significantly improves treatment outcomes. This project builds an AI-powered screening tool that classifies kidney CT scan images as either **Tumor** or **Normal** using two trained deep learning models:

- A **custom CNN** (`custom_cnn_model.h5`)
- A **VGG-based transfer learning model** (`model_vgg.h5`)

The Streamlit web app provides an accessible, user-friendly interface where medical professionals or patients can upload CT images and get an instant prediction along with a confidence score.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| TensorFlow / Keras | CNN and VGG model training and inference |
| Streamlit | Interactive web application UI |
| Pillow (PIL) | Image loading and preprocessing |
| NumPy | Array manipulation |
| Jupyter Notebook | Model training and experimentation |

---

## 📁 Project Structure

```
├── Final_web_code.py                              # Streamlit web app for CT scan classification
├── Kidney_tumor_classification_using_deeplearning.ipynb  # Model training notebook
├── custom_cnn_model.h5                            # Trained custom CNN model
├── model.h5                                       # Alternative saved model
├── model_vgg.h5                                   # Trained VGG transfer learning model
├── cancerimage.jpeg                               # Sample tumor CT scan image
├── normalimage.jpeg                               # Sample normal CT scan image
├── images/                                        # Additional sample images
└── README.md                                      # Project documentation
```

---

## ⚙️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/priya-zha/Kidney-Tumor-Classification.git
cd Kidney-Tumor-Classification
```

### 2. Install Dependencies
```bash
pip install tensorflow keras streamlit pillow numpy
```

### 3. Update Model Path
In `Final_web_code.py`, update the model path to your local path:
```python
model = load_model("model_vgg.h5")  # update path if needed
```

### 4. Run the Streamlit App
```bash
streamlit run Final_web_code.py
```

---

## 🚀 Usage

1. Open the app in your browser at `http://localhost:8501`
2. Read the informational section about kidney cancer
3. Upload a CT scan image (`.jpeg`, `.jpg`, or `.png`)
4. Click the **Detect** button
5. The app will display:
   - **Tumor** — if a kidney tumor is detected, along with the confidence score
   - **Normal** — if no tumor is detected

---

## 📓 Notebook

The `Kidney_tumor_classification_using_deeplearning.ipynb` notebook contains the full model training pipeline including data loading, augmentation, custom CNN architecture, VGG transfer learning setup, training, and evaluation.

---

## 📋 Requirements

- Python 3.8+
- TensorFlow 2.x / Keras
- Streamlit
- Pillow
- NumPy

---

## 👩‍💻 Author

**Priya** — [@priya-zha](https://github.com/priya-zha)
