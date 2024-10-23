
---

# Hyperspectral Image Classification using Swin Transformer

This repository contains code for **HSI (Hyperspectral Image) classification** using the **Swin Transformer** architecture, applied to the **Pavia University dataset**. The approach can easily be adapted to other HSI datasets by changing the dataset paths.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Model](#model)
- [Setup](#setup)
- [Usage](#usage)
- [Results](#results)
- [Customization](#customization)


---

## Introduction
Hyperspectral imaging (HSI) is an essential technique for remote sensing, capable of capturing hundreds of spectral bands for each pixel. The Swin Transformer, a modern transformer-based architecture, is leveraged here for efficient HSI classification. This project demonstrates how to perform HSI classification using **the Pavia University dataset** and allows for easy switching to other datasets.

---

## Dataset
The default dataset used in this project is the **Pavia University dataset**, a widely-used hyperspectral dataset for remote sensing applications.

- **Download the Dataset**: [Pavia University Dataset](http://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes#Pavia_University_scene)
- **Dimensions**: 610 × 340 pixels, 103 spectral bands

You can also replace the dataset with other HSI datasets. Ensure that the new dataset is preprocessed to match the input shape required by the model.

---

## Model
The model used for this task is the **Swin Transformer**, a state-of-the-art transformer architecture originally designed for vision tasks. The hierarchical structure of the Swin Transformer enables it to capture local and global dependencies efficiently, making it suitable for HSI classification.

---

## Setup

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure you have access to the dataset. You can place the dataset files in a folder named `data/` by default.

---

## Usage

1. **Run the notebook:**
   Open the `PaviaUniversity_HSI.ipynb` file in Jupyter or any compatible notebook environment.

2. **Change Dataset:**  
   To use a different dataset, modify the paths in the notebook under the data loading section:
   ```python
   dataset_path = "/path/to/your/new/dataset"
   ```

3. **Training the model:**
   The notebook contains steps for:
   - Data loading and preprocessing
   - Model initialization
   - Training and evaluation

4. **Results:**  
   After training, you can view the accuracy, precision, recall, and confusion matrix for both training and validation datasets.

---

## Results
With the **Pavia University dataset**, you can expect competitive classification performance using the Swin Transformer. Results will vary depending on the dataset, training epochs, and hyperparameters used.

---

## Customization
- **Changing the Dataset:** Update the dataset path in the notebook to switch datasets.
- **Hyperparameter Tuning:** You can experiment with learning rates, epochs, batch sizes, and optimizer settings in the training section of the notebook.
- **Model Modifications:** Modify the model architecture or use different transformer blocks as needed.

---



---

## Acknowledgments
Reference
This implementation draws inspiration from  the SpectralFormer as our base paper.

SpectralFormer Paper:
-**Title:** SpectralFormer: Rethinking Hyperspectral Image Classification with Transformers.
-**Authors:** Danfeng Hong, Zhu Han, Jing Yao, Lianru Gao, Bing Zhang, Antonio Plaza, and Jocelyn Chanussot.
-**Link:** https://arxiv.org/abs/2107.02988.
-**Publication:** IEEE Transactions on Geoscience and Remote Sensing.



