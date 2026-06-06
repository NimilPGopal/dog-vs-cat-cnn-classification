# Dog vs Cat Classification using CNN

## Project Overview

This project implements an Image Classification System using Convolutional Neural Networks (CNN) to classify images as either Dog or Cat.

The model was trained using TensorFlow and Keras and evaluated using training and validation accuracy/loss metrics.

---

## Dataset

The dataset used for this project is the Dogs vs Cats image dataset.
Dataset is not included in this repository due to size limitations.

* Binary Classification Problem
* Image Size: 64 × 64

---

## CNN Architecture

```text
Conv2D (32 Filters)
↓
MaxPooling2D
↓
Conv2D (64 Filters)
↓
MaxPooling2D
↓
Flatten
↓
Dense (128)
↓
Output Layer
```

### Model Summary

| Layer        | Output Shape |
| ------------ | ------------ |
| Conv2D       | (62,62,32)   |
| MaxPooling2D | (31,31,32)   |
| Conv2D       | (29,29,64)   |
| MaxPooling2D | (14,14,64)   |
| Flatten      | 12544        |
| Dense        | 128          |
| Output       | 1            |

Total Parameters: **1,626,442**

---

## Model Performance

| Metric | Value |
|----------|---------|
| Training Accuracy | 84.75% |
| Validation Accuracy | 84.87% |
| Training Loss | 0.3599 |
| Validation Loss | 0.3469 |

---

## Sample Predictions

### Cat Prediction

Model correctly predicted:

```text
Prediction: Cat
```

### Dog Prediction

Model correctly predicted:

```text
Prediction: Dog
```

---

## Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib
* Jupyter Notebook

---

## How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/NimilPGopal/dog-vs-cat-cnn-classification.git
cd dog-vs-cat-cnn-classification
```

### 2. Create a Virtual Environment

**Windows**

```bash
python -m venv venv
```

**Linux / macOS**

```bash
python3 -m venv venv
```

### 3. Activate the Virtual Environment

**Windows (CMD)**

```bash
venv\Scripts\activate
```

**Linux / macOS**

```bash
source venv/bin/activate
```


### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
notebooks/cnnRunCode.ipynb
```

### 6. Run the Project

Execute all notebook cells to:

* Load the dataset
* Train the CNN model
* Visualize training and validation metrics
* Save the trained model
* Test predictions on new images

### 7. Deactivate Virtual Environment

When finished:

```bash
deactivate
```

---

**Project Structure** 

```text
dog-vs-cat-cnn-classification/
│
├── models/
│   ├── cnn_model3.keras
│   └──cnn_model4.keras
│
├── notebooks/
│   └── cnnRunCode.ipynb
│
├── results/
│   └── model_summary.png
│
├── logs/
│   └── log.csv
││
├── requirements.txt
├── README.md
└── .gitignore
```
