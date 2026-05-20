# 🧠 Brain Tumor Segmentation using U-Net in TensorFlow  

This project implements a deep learning-based **semantic segmentation model** to identify and segment brain tumors from MRI scans. Using a **U-Net architecture**, the model learns to distinguish tumor regions from the background in medical images.  

---

## 📖 Project Overview  

| Feature        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| 🎯 Goal        | Accurately segment tumor regions from brain MRI images using deep learning |
| 📂 Dataset     | Brain tumor segmentation dataset with paired images and masks              |
| 🏗️ Architecture | U-Net convolutional neural network implemented in TensorFlow/Keras         |
| 💻 Platform    | Developed locally in **VS Code** with GPU support                          |

---

<p align="center">
  <img src="screenshots/confusion-matrix.png" width="700">
</p>

<p align="center">
  Confusion matrix generated from U-Net based MRI brain tumor segmentation evaluation.
</p>

## 🚀 Technologies Used  

- **TensorFlow / Keras** – Building and training the deep learning model  
- **OpenCV** – Image processing and data preparation  
- **Scikit-learn** – Evaluation metrics and model validation  
- **Matplotlib / Seaborn** – Visualization of training progress and results  

---

## 📊 Model Evaluation  

The model was trained for **10 epochs** and evaluated on a held-out **test set**.  

| Metric            | Value   |
|-------------------|---------|
| ✅ Accuracy        | 98.27%  |
| 🎯 Precision      | 0.5591  |
| 🔍 Recall         | 0.7076  |
| 📐 F1 Score       | 0.6247  |
| 📊 AUC-ROC Score  | 0.8492  |

---

## 📌 Confusion Matrix  

|                       | Predicted Negative | Predicted Positive |
|-----------------------|-------------------:|-------------------:|
| **Actual Negative**   | 39,150,709         | 366,303            |
| **Actual Positive**   | 191,962            | 464,594            |

---

## 📂 Project Structure  

```
Brain_Tumor_Segmentation_Using_U-NET/
│── data/                 # Dataset (MRI scans + masks)
│── notebooks/            # Jupyter notebooks for experiments
│── src/                  # Source code for training + model
│   ├── model.py          # U-Net implementation
│   ├── train.py          # Training loop
│   ├── evaluate.py       # Evaluation script
│── results/              # Saved outputs (plots, predictions)
│── requirements.txt      # Dependencies
│── README.md             # Project documentation
```

---

## ⚡ How to Run  

1. Clone this repo:  
   ```bash
   git clone https://github.com/SayedMohamedSaqib/Brain_Tumor_Segmentation_Using_U-NET.git
   cd Brain_Tumor_Segmentation_Using_U-NET
   ```

2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```

3. Train the model:  
   ```bash
   python src/train.py
   ```

4. Evaluate the model:  
   ```bash
   python src/evaluate.py
   ```

---

## 📜 License  

This project is licensed under the **MIT License** – feel free to use and modify.  
