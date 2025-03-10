# Lab 1: Deep Learning 

## Project Overview

Welcome to **Lab 1: Deep Learning Unleashed**, my submission for the Deep Learning course! This project showcases two killer applications of neural networks:

- **Regression**: Predicting NYSE stock closing prices using a DNN, with regularization to keep overfitting in check.
- **Classification**: Detecting machine failures with a DNN classifier, optimized via grid search and beefed up with dropout.

Built with **PyTorch** on Google Colab, this repo is a testament to data wrangling, model crafting, and performance tuning—all in one slick Jupyter Notebook.

## Features

-  **NYSE Regression**: Predicts stock prices using a 3-layer DNN (3-64-32-1) with ReLU and dropout.
-  **Maintenance Classification**: Classifies machine failures (binary) with a tuned DNN (7-64-32-2).
-  **Data Viz**: Histograms, scatter plots, loss/MAE/accuracy curves—visuals that pop!
-  **Regularization**: Dropout (0.2) and weight decay (0.01) to fight overfitting like a boss.
-  **GPU Power**: Leverages CUDA for lightning-fast training.
-  **Hyperparameter Tuning**: Grid search over learning rates and optimizers for peak performance.

---

## Requirements

To run this beast, you'll need:

- **Python 3.8+**
- **Jupyter Notebook** (or Colab)
- **Dependencies:**

```bash
torch==2.0.1
pandas==2.0.3
numpy==1.24.3
matplotlib==3.7.1
seaborn==0.12.2
scikit-learn==1.3.0
imblearn==0.11.0
kagglehub
```

- **Optional**: GPU with CUDA for max speed.

---

##  Installation

### Clone the Repo:
```bash
git clone https://github.com/badrbenabdellah/Deep_Learning_Workshop1
cd Atelier1
```


---

## Usage

### 1. Open the Notebook:
- Fire up **lab1_deep_learning.ipynb** in Jupyter or upload it to Google Colab
### 2. Run It:
- Hit **Run All** (or `Shift + Enter` cell-by-cell) to:
  - 📥 Download datasets via **kagglehub**.
  - 🔄 Preprocess, train, and evaluate both models.
  - 📊 Generate dope plots.

### 3. Outputs:
- Check inline plots (loss, MAE, accuracy) and printed metrics (accuracy, sensitivity, F1-score).

💡 **Pro Tip**: Got a **GPU**? Colab’s free CUDA support will make this fly!

---

## Results

NYSE Regression
 -  Task: Predict closing prices from open, high, and low.
 -  Model: DNN (3-64-32-1) + ReLU + Dropout (0.2).
 -  Loss: MSE dropped from 12,062 to 16.55 (regularized) over 100 epochs.
 -  MAE: Slashed to ~4.0 on test set with regularization.
 -  Takeaway: Dropout and weight decay crushed overfitting—test loss stayed tight!

 -  ![image](https://github.com/user-attachments/assets/d872078c-079d-4395-b087-6729ec6cad7b)
 -  ![image](https://github.com/user-attachments/assets/aa8f28f4-413a-484f-bb4c-1becc7ecce3c)


**Maintenance Classification**   
 -  Task: Predict machine failure (Target: 0 or 1).
 -  Model: DNN (7-64-32-2) + ReLU + Dropout (0.2).
 -  Best Params: lr=0.01, optimizer=adam (via grid search).
 -  Metrics:
     -  Accuracy: 95.47%
     -  Sensitivity: 96.84%
     -  F1 Score: 95.53%
     -  Takeaway: SMOTE balanced the classes, and regularization kept generalization solid.

---

![image](https://github.com/user-attachments/assets/06f376ce-3400-4a65-98d6-383328777911)
![image](https://github.com/user-attachments/assets/c7200d08-373c-43d9-be76-b6de19a15ec0)

