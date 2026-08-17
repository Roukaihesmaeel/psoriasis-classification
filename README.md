# Psoriasis Classification Using Deep Learning

An AI-based deep learning project for classifying skin images into **Psoriasis** and **Normal Skin** using **MobileNetV2** and TensorFlow/Keras.

## Project Overview

This project aims to demonstrate how deep learning can be applied to skin image classification.

The model was trained on a psoriasis dataset containing approximately **10,000 images** divided into two classes:

* **Normal Skin:** 4,099 images
* **Psoriasis:** 5,908 images

## Technologies

* Python
* TensorFlow / Keras
* MobileNetV2
* NumPy
* Pillow
* Gradio
* Google Colab

## Model Architecture

The project uses **MobileNetV2** pretrained on ImageNet as the base model.

The classification architecture includes:

* MobileNetV2
* Global Average Pooling
* Dense layer with 128 neurons
* Dropout
* Binary classification output using Sigmoid

## Image Preprocessing

The images were processed using several techniques, including:

* Resizing to 224 × 224
* LAB color space conversion
* CLAHE
* Gaussian Blur

## Training

The model was initially trained with the MobileNetV2 base layers frozen, followed by fine-tuning using a lower learning rate.

The model achieved approximately **98.8% validation accuracy** during training.

> This project is an educational AI prototype and is not intended to provide medical diagnosis.

## Demo

A web-based demo of the trained model is available on Hugging Face:

**Psoriasis Classifier:**
https://huggingface.co/spaces/roukaih/psoriasis-classifier

## Project Files

* `psoriasis_classification.ipynb` — Google Colab notebook containing the project code and training workflow.
* `requirements.txt` — Python dependencies.
* `.gitignore` — Files excluded from version control.

## Future Improvements

* Expand the model to classify multiple skin diseases.
* Add Explainable AI techniques such as Grad-CAM.
* Improve dataset diversity and model generalization.
* Deploy an improved version as a web application.

## Author

**Roukaih Esmaeel**

AI / Information Engineering
