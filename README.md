# t5-prompt-regen

This repository contains the Jupyter Notebook and associated files for the "Prompt Prediction with T5" project. The aim of this project is to train a T5 (Text-to-Text Transfer Transformer) model to accurately predict the original prompts from rewritten text versions. This involves developing a model that can understand and reverse-engineer the rewriting process, thus revealing the initial queries that generated specific textual outputs.


## Data Collection and Preparation
### Data Sources:
The dataset used to train the T5 model consists of texts derived from a combination of the following sources:

**Brown Corpus:** Sections of the corpus were segmented into chunks containing 80-128 tokens to form the base for training data.
**Web Scraping:** Additional texts were gathered through web scraping techniques to diversify the data pool and enhance model robustness.
**Synthetic Data:** To further expand the dataset, synthetic texts were generated using advanced language models including Google Gemini and ChatGPT.

### Data Processing:

The collected data underwent several preprocessing steps to optimize it for training:

**Tokenization:** Texts were tokenized according to the model’s requirements.
**Segmentation**: Data from the Brown Corpus was segmented to ensure uniformity in text length across the dataset.

## Feature Enhancement:
To enrich the dataset and improve the model's prediction accuracy, additional linguistic features were incorporated:

**Cosine Similarity:** This metric was calculated between various text pairs to quantify the semantic similarity, aiding the model in understanding nuanced differences and similarities in context.
**Sentiment Polarity:** Each text segment was annotated with sentiment scores to capture the emotional tone, providing the model with deeper contextual insights.

## Model Training and Evaluation
The T5 model is trained using the enhanced dataset, focusing on its ability to predict original prompts from rewritten text. Training involves several iterations to fine-tune the model's parameters for optimal performance. The evaluation is conducted using a held-out test set to ensure the model's accuracy and ability to generalize across unseen data.

# Usage
To replicate the training process or to use the model for your text rewriting tasks:

- Navigate to the Notebooks directory.
- Open the Training.ipynb notebook.
- Follow the instructions within the notebook to setup your environment and run the cells.
