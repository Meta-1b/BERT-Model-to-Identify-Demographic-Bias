# Finetuning LLM to Identify Demographic Bias

We'd like to thank all the Meta collaborators we worked with throughout this process-- particularly our challenge Advisor Megan and TA Grace.

## Project Overview

Our project focused on three main goals:

- Training an LLM to assess demographic bias in datasets
- Preprocessing models and finetuning pre-trained BERT model from HuggingFace Hub
- Building a documented pipeline/tool for model evaluation

Biased chatbots can reinforce harmful sterotypes that negatively impact the way we view individuals in society and even historical events. It may limit opportunities and perpetuate harmful gender role perceptions. LLMs such as ChatGPT and Llama have the potential to learn from biased datasets-- narrowing their perception of particular groups of individuals specific to bias or incorrect information.

## Preprocessing

- We utilized the RedditBias dataset and focusing specifically on csv files containing the 'annotated' key word
- Data cleaning and feature engineering
- Combined all datasets into one larger dataframe creating another column specific for the bias type before converting to csv file to upload to the HuggingFace Hub

## Model Development

- Splitting into testing, training, and evaluation datasets through HuggingFace Hub
- Imported BERT model
- Training (text classification model)

## Evaluation

- Evaluation through 'evaluate' class
- Accuracy of 43.5%
- Hyperparameter Tuning through Optuna Backend and Trainer API

## Next Steps

- Hyperparameter tuning 
