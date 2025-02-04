## 🚀PFA-projet IoT Schema Generation from Text (IoT GPT)
Automated IoT schema generation using NLP & NER, accelerating IoT system design from textual descriptions.

## 🌍Context

This project aims to automate IoT schema generation from text using NLP techniques like Named Entity Recognition (NER). It enhances efficiency in IoT system design by extracting IoT-related entities from unstructured descriptions.

## 📌Project Description

This project focuses on extracting IoT-specific entities from textual descriptions using NLP techniques, particularly NER (Named Entity Recognition). The extracted entities are structured to facilitate automatic IoT schema generation.
## 📂Repository Structure

### 1️⃣Dataset

This folder contains datasets used for training and testing the NER model:
- NER_iob.csv: Dataset annotated in IOB format for NER model training.
- iot_comp.csv: List of extracted IoT components.
- melted_data.csv: Transformed version of data for better model compatibility.
- ner_dataset.txt: Raw text file containing sentences used for training.
- test_data.txt: Test data for evaluating model performance.
- testNER.csv: Formatted test data for NER model validation.
  
### 2️⃣Preprocessing dataset
This folder contains scripts for data preprocessing:
- iot_gpt_clean.ipynb: Notebook for data cleaning and preparation before model training.

### 3️⃣Training model
This folder includes notebooks for training various NER models:
- training_CRF_Bi_LSTM.ipynb: Notebook for training a Conditional Random Fields (CRF) + Bi-LSTM based NER model.
- training_pre_trained_model.ipynb: Notebook utilizing a pre-trained model (e.g., BERT, spaCy) for IoT entity extraction.

## 📂Key Steps

**📊Data Collection:** Web scraping + manual dataset combination.<br>
**🧹 Preprocessing:** Tokenization, normalization, stop words & abbreviation handling.<br>
**🔍 Entity Extraction:** Using SpaCy & PhraseMatcher to identify IoT components.<br>
**🤖 Model Training:** Testing BERT, DistilBERT, RoBERTa, and CRF + Bi-LSTM with early stopping & class balancing.<br>
**🔮 Future Work:** Automating IoT schema generation from extracted entities.<br>
