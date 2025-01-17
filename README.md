# EthioMart - Telegram-Based E-Commerce Hub (NER System for Amharic)

## Overview

EthioMart aims to centralize Ethiopian-based Telegram e-commerce channels into a unified platform. This project focuses on fine-tuning a Named Entity Recognition (NER) system to extract key business entities (e.g., product names, prices, locations) from messages, images, and documents shared across Telegram channels. The extracted data will be used to populate EthioMart's centralized database, making it a comprehensive e-commerce hub.

## Key Objectives
- Real-time data extraction from Telegram channels
- Fine-tune LLMs to extract product names, prices, and locations from Amharic text.

## Data Sources
- **Telegram Channels**: Data from Ethiopian-based e-commerce Telegram channels.
- **Types**: 
  - Text (Amharic messages)
  - Images (Product images, marketing materials)

## Setup Instructions

### Requirements
- Python 3.x
- Libraries:
  - `transformers`
  - `datasets`
  - `torch`
  - `pandas`
  - `numpy`
  - `sklearn`

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/1Light/kaim-week-5.git
   cd kaim-week-5
   ```
2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Data Collection
1. Use a custom scraper to collect messages from selected Telegram channels.
2. Preprocess and clean the data for entity extraction.

### Fine-Tuning the Model
1. Fine-tune a multilingual model like `XLM-Roberta` or `BERT-tiny-Amharic` on labeled CoNLL data.
2. Use Hugging Face's Trainer API to train the NER model.

## Results & Evaluation
- Evaluate models based on accuracy and speed.
- Select the best-performing model for production.

## License
MIT License - see the [LICENSE](LICENSE) file for details.