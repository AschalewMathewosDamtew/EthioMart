# EthioMart Amharic NER System

## Project Overview

EthioMart aims to consolidate real-time e-commerce data from multiple Ethiopian-based Telegram channels into a single platform. This project focuses on fine-tuning a Named Entity Recognition (NER) system to extract key business entities such as **product names**, **prices**, and **locations** from text, images, and documents shared in Amharic across these channels.

The extracted data will populate EthioMart's centralized database, providing a streamlined experience for customers and vendors alike.

## Key Objectives

1. **Real-time Data Extraction**: Extract messages, images, and documents from various Telegram e-commerce channels.
2. **NER Fine-tuning**: Fine-tune pre-trained models (XLM-Roberta, bert-tiny-amharic, or afroxmlr) for extracting key entities from Amharic text.
3. **Model Comparison**: Evaluate and select the best-performing model using metrics like F1-score, precision, and recall.
4. **Model Interpretability**: Use SHAP and LIME to interpret and explain the model’s decisions.


## Tasks Breakdown

### 1. Data Ingestion & Preprocessing
- Ingest text, images, and documents from Telegram e-commerce channels.
- Preprocess Amharic text by tokenizing, normalizing, and handling linguistic features.
- Structure data and store it in a unified format.

### 2. Labeling Dataset in CoNLL Format
- Label messages for **Product**, **Price**, and **Location** entities.
- Save labeled data in CoNLL format.

### 3. Fine-tune NER Models
- Fine-tune models such as **XLM-Roberta**, **bert-tiny-amharic**, and **afroxmlr** for extracting entities.
- Tokenize the data and align the labels with the tokenized output.
- Train using Hugging Face’s **Trainer API**.

### 4. Model Comparison & Selection
- Fine-tune multiple models and evaluate performance using metrics like F1-score.
- Compare the performance and select the best-performing model for production.

### 5. Model Interpretability
- Use **SHAP** and **LIME** to explain model predictions and decisions.
- Analyze difficult cases where the model struggles to correctly identify entities.

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/AschalewMathewosDamtew/EthioMart.git