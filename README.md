# End-to-End Bank Administrative Assistant

This repository contains an end-to-end project developed to assist bank managers in analyzing customer feedback, summarizing key insights, and generating actionable solution scenarios.  

## Project Overview  

The project focuses on:  
1. **Classifying customer complaints** using advanced NLP models.  
2. **Summarizing grouped data** for concise representation.  
3. **Providing solution scenarios** for managerial decision-making.  

## Dataset  

The dataset used for this project is the [banking77 dataset](https://huggingface.co/datasets/legacy-datasets/banking77), which includes labeled customer complaints for banking-related issues.  

## Steps and Workflow  

### 1. Classification Models  

#### a) SpaCy Model  
- Fine-tuned the `en_core_web_trf` model to classify customer complaints effectively.  

#### b) BERT Model  
- Trained the [google-bert/bert-base-uncased](https://huggingface.co/google/bert-base-uncased) model.  
- The fine-tuned model was uploaded to Hugging Face as [BERT-BankingClassifier](https://huggingface.co/saribasmetehan/BERT-BankingClassifier).  
- Integrated the model into a pipeline for easy inference.  

### 2. Data Grouping  

Customer complaints were grouped based on their labels to facilitate targeted analysis.  

### 3. Summarization  

Used the `philschmid/bart-large-cnn-samsum` model to summarize grouped data for concise insights.  

### 4. Solution Scenarios  

Implemented the `microsoft/Phi-3-mini-4k-instruct` model to generate actionable solutions tailored for bank managers.  

