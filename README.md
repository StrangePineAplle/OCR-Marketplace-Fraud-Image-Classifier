# OCR-Marketplace-Fraud-Image-Classifier

# Marketplace Fraud Detection with EasyOCR and RuBERT

## Overview
The **Marketplace Fraud Detection with EasyOCR and RuBERT** project aims to identify fraudulent images in online marketplaces by classifying them into two categories: fraud and non-fraud. The model focuses on detecting images that contain deceptive text, such as scam messages, to enhance trust and safety in e-commerce environments.

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
