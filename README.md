# Relation-Extraction-in-NLP-using-Deep-Learning-Models



This project provides two approaches for relation extraction classification using deep learning and machine learning techniques.

## Project Overview

- **Approach 1:** Deep Learning using Neural Networks
- **Approach 2:** Machine Learning using Support Vector Machines (SVM) with Stacking Classifier

Both approaches are implemented in Python and can be executed on **Google Colab**.

## Setup and Usage in Google Colab

### 1. Open the Python Notebooks
You can open the provided Python notebooks in Google Colab for training and testing the models:
- `Final_Neural_Networks_Model.pynb`
- `Final_StackingClassifier_Model.ipynb`

### 2. Required Steps
Once you open the Colab notebooks, follow these steps:

#### 2.1 Install Dependencies
Execute the cells one by one to install the required libraries and load the necessary functions.

#### 2.2 Upload Necessary Files
- **glove.6B.100d.txt** for the neural-based approach:
  - Download the GloVe embeddings file from the link below:
    [GloVe Embeddings](https://drive.google.com/drive/folders/1elk41Qhy-ppaZpbeabfiXhoEMO9BLvg5?usp=sharing)
  - Upload it in the Colab runtime under the "Files" section.

- **classifier.py** for both approaches:
  - Upload the `classifier.py` file to the Colab environment. This file is already included in the project folder. You can either upload it directly or use a cloud storage link.

## Model Training and Testing

### 1. Deep Learning Approach (Neural Networks)
- **Enable GPU Acceleration:** Ensure you have **T4 GPU** enabled in Colab for faster training.
- Execute the cells in the `Final_Neural_Networks_Model.pynb` to train the deep learning model.
- Use the same notebook for testing and user-testing.

### 2. Machine Learning Approach (SVM with Stacking Classifier)
- Execute the cells in the `Final_StackingClassifier_Model.ipynb` to train and test the SVM-based model.
- For faster user-testing compilation, you can also use the `Final_StackingClassifier_UserTesting.ipynb` notebook.

## User Testing

### After Training:
For classifying new sentences after model training, use the `classifier.py` module. Follow these import statements for each approach:

- **For Deep Learning Approach:**
  ```python
  from classifier import classify_relation
  ```

- **For SVM Approach:**
  ```python
  from classifier import classify_relation_svm
  ```
