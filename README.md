# Multimodal IMDb Genre Classification with Keras

## Overview

This project explores a multimodal approach to movie genre classification using both visual and textual data from IMDb.

Each film in the dataset contains:
- A movie poster image
- A textual movie overview
- One or more genre labels

Because a film can belong to multiple genres at the same time, this project is framed as a multi-label classification problem.

The project compares two deep learning models:

- A Convolutional Neural Network (CNN) for poster-based genre classification
- A Bidirectional LSTM model for overview-based genre classification

The aim is to evaluate how well visual and textual features contribute to genre prediction.

---

## Project Objectives

- Preprocess image and text data for deep learning
- Build and train a CNN model for movie poster classification
- Build and train a Bidirectional LSTM model for movie overview classification
- Compare model performance using training and validation metrics
- Analyse model behaviour, including overfitting, class imbalance, and prediction patterns

---

## Models Used

### CNN Model

The CNN model was trained on movie poster images. It uses convolutional layers to extract visual patterns from posters and predict movie genres.

### LSTM Model

The LSTM model was trained on movie overview text. It uses embedding and bidirectional LSTM layers to learn semantic patterns from descriptions.

---

## Key Findings

- The CNN model showed more stable training and better generalisation.
- The LSTM model learned meaningful patterns from text but showed signs of overfitting.
- Both models struggled with class imbalance.
- Popular genres such as Drama and Comedy were more frequently predicted.
- The results highlight the difficulty of multi-label genre classification.

---

## Repository Structure

```text
multimodal-imdb-genre-classification-keras/
│
├── notebook/
│   └── multimodal_imdb_genre_classification.ipynb
│
├── report/
│   └── multimodal_imdb_genre_classification_report.pdf
│
├── images/
│   └── sample_outputs.png
│
├── README.md
│
└── requirements.txt
