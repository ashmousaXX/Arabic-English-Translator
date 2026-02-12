# Arabic-English-Translator
# Arabic-to-English Neural Machine Translation with Transformer

This repository contains an **Arabic-to-English Neural Machine Translation (NMT)** system implemented with a **Transformer architecture**. The project includes **data preprocessing, tokenization, training, evaluation, and a web-based GUI** for real-time translations.  

## Overview

This project implements a **full NMT pipeline** for translating Arabic sentences to English using the **Transformer model**. It includes:

1. **Data Preprocessing**: Cleaning Arabic and English text, removing unwanted characters, normalizing Arabic text, and splitting data into train/validation/test sets.  
2. **Tokenization**: Using **SentencePiece** to generate subword vocabularies for both Arabic and English.  
3. **Transformer Model**: Custom implementation with **encoder, decoder, positional encoding, and attention masks**.  
4. **Training**: Training with a custom learning rate scheduler and gradient clipping.  
5. **Evaluation**: BLEU score calculation using **sacreBLEU** for both greedy and beam search decoding.  
6. **GUI**: Interactive **Gradio** interface to translate Arabic sentences in real-time and maintain a translation history.
   
## Features

- Custom preprocessing for Arabic (diacritics removal, Alef normalization, and punctuation filtering).  
- Tokenization using **Byte-Pair Encoding (BPE)** with **SentencePiece**.  
- Transformer-based sequence-to-sequence model with **multi-head attention** and **positional encoding**.  
- Supports **greedy decoding** and **beam search** for improved translation.  
- BLEU score evaluation for quantitative performance measurement.  
- Interactive **Gradio GUI** with translation history and clearable interface.  

## Dataset

The project uses the dataset from [Samir Moustafa's GitHub repository](https://github.com/SamirMoustafa/nmt-with-attention-for-ar-to-en):

- File: `ara_.txt`  
- Format: Tab-separated Arabic–English sentence pairs.  
- Preprocessing includes:
  - Cleaning Arabic and English text.
  - Filtering sentences by length (2–80 words).
 
    


## Installation

Clone the repository and install required dependencies:

```bash
git clone https://github.com/ashmousaXX/arabic-nmt-transformer.git
cd arabic-nmt-transformer
pip install -r requirements.txt

