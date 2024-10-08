# Bilingual Sexism Classification: Fine-Tuned XLM-RoBERTa and GPT-3.5 Few-Shot Learning

This repository contains the code and resources for the paper titled "Bilingual Sexism Classification: Fine-Tuned XLM-RoBERTa and GPT-3.5 Few-Shot Learning," presented at the EXIST Lab at CLEF 2024. This work aims to improve sexism identification in bilingual contexts (English and Spanish) by leveraging natural language processing models.

## Table of Contents
- [Introduction](#introduction)
- [Methodology](#methodology)
- [Dataset](#dataset)
- [Results](#results)

## Introduction

Sexism in online content is a pervasive issue that necessitates effective classification techniques to mitigate its harmful impact. Our study aims to improve sexism identification by fine-tuning the XLM-RoBERTa model and using GPT-3.5 with few-shot learning prompts to classify sexist content. We participated in the EXIST 2024 challenge and achieved notable results in both sexism identification and source intention detection tasks.

## Methodology

### Fine-Tuning XLM-RoBERTa
- **Model:** XLM-RoBERTa, an advanced version of RoBERTa trained on 100 languages.
- **Hyper-Parameter Tuning:** Optimized parameters including learning rate, weight decay, and number of epochs.
- **Optimization:** Used AdamW optimizer with early stopping and a dynamic learning rate scheduler.

### Few-Shot Learning with GPT-3.5
- **Prompt Design:** Employed few-shot learning with randomly selected English and Spanish tweets from the training dataset.
- **Model Execution:** Focused on extracting hard labels from the outputs.
- **Evaluation:** Performance evaluated using accuracy and metrics tailored for multilingual input.

## Dataset

The EXIST 2024 dataset is composed of more than 10,000 tweets in English and Spanish, divided into training, development, and test sets. Each tweet is annotated with demographic parameters of the annotators and labels indicating whether the tweet is sexist and the intention behind it.

## Results

Our approach using XLM-RoBERTa achieved 4th place in the soft-soft evaluation of Task 1 (sexism identification) and 2nd place in the soft-soft evaluation of Task 2 (source intention). Detailed results and performance metrics are provided in the [paper](https://ceur-ws.org/Vol-3740/paper-89.pdf).
