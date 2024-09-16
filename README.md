# OCR-Marketplace-Fraud-Image-Classifier
![Python](https://img.shields.io/badge/python-v3.6+-blue.svg)
![CLIP](https://img.shields.io/badge/EasyOCR-green)
![CatBoost](https://img.shields.io/badge/RuBERT-yellow)

[![OCR base solution](https://img.shields.io/badge/CLIP%20base%20solution%20-%20red)](https://github.com/StrangePineAplle/CLIP-Marketplace-Fraud-Image-Classifier)

## Overview
The **Marketplace Fraud Detection with EasyOCR and RuBERT** project aims to detect fraudulent images in online marketplaces by classifying them as either fraudulent or non-fraudulent. The model is trained to identify images that contain deceptive text, such as "деньги за отзывы телеграм @mony_tg," which are commonly associated with scams.
## Data

The dataset used for training the **Marketplace Fraud Image Classifier** consists of two main categories: fraudulent images and non-fraudulent (normal) images.

### Fraudulent Images
The fraudulent data examples contain images that feature deceptive text, such as scam messages or suspicious offers. These images are crucial for training the model to accurately identify potential fraud attempts. Some examples of fraudulent images are shown below:

<p align="left">
  <img src="https://github.com/StrangePineAplle/OCR-Marketplace-Fraud-Image-Classifier/blob/main/pictures/fraud1.jpg" width="200" />
  <img src="https://github.com/StrangePineAplle/OCR-Marketplace-Fraud-Image-Classifier/blob/main/pictures/fraud2.jpg" width="200" /> 
</p>

### Non-Fraudulent (Normal) Images
The non-fraudulent data examples represent legitimate images that do not contain any suspicious content. These images serve as a contrast to the fraudulent data, helping the model distinguish between genuine and fraudulent listings. Examples of non-fraudulent images are provided below:

<p align="left">
  <img src="https://github.com/StrangePineAplle/OCR-Marketplace-Fraud-Image-Classifier/blob/main/pictures/norm1.jpg" width="200" />
  <img src="https://github.com/StrangePineAplle/OCR-Marketplace-Fraud-Image-Classifier/blob/main/pictures/norm2.jpg" width="200" />
</p>

By training the model on a balanced dataset consisting of both fraudulent and non-fraudulent images, the **Marketplace Fraud Image Classifier** can learn to effectively distinguish between legitimate and suspicious content, ultimately enhancing the safety and trust in online marketplaces.

## Model Architecture

### EasyOCR
EasyOCR (Easy Optical Character Recognition) is a powerful library for extracting text from images. It supports a wide range of languages and is known for its accuracy and ease of use. In this project, EasyOCR is employed to extract text from the input images.

### Sage
Sage is a grammar correction library that helps improve the quality of extracted text. It analyzes the text and suggests corrections based on grammatical rules and context. By integrating Sage, the project ensures that the extracted text is grammatically correct and easier to process for further analysis.

### RuBERT
RuBERT (Russian BERT) is a pre-trained language model based on BERT (Bidirectional Encoder Representations from Transformers). It is specifically designed for the Russian language and is trained on a large corpus of Russian text. RuBERT is used in this project for understanding the meaning of the extracted text and classifying it as either fraudulent or non-fraudulent.

## Features
- **Text Extraction**: EasyOCR is used to extract text from input images.
- **Grammar Correction**: Sage is employed to correct grammatical errors in the extracted text.
- **Text Understanding**: RuBERT is utilized to understand the meaning of the corrected text and classify it as either fraudulent or non-fraudulent.
- **Fraud Detection**: The model identifies fraudulent images based on the extracted and analyzed text.

## Results

The performance of the **Marketplace Fraud Image Classifier** was evaluated using various metrics, with a primary focus on the F1 score, which balances precision and recall. 

After thorough training and validation, the final model achieved an impressive F1 score of **0.92**. This high score indicates that the model is highly effective in distinguishing between fraudulent and non-fraudulent images, demonstrating its ability to minimize false positives and false negatives.

### Performance Metrics
- **F1 Score**: 0.96
- **speed**: more then 5 minute/3000 img

