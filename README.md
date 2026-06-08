# AI-powered-paraphrasing-tool
AI-powered paraphrasing system using T5, LanguageTool, and Sentence-BERT. Includes grammar correction, semantic similarity scoring, BLEU/ROUGE evaluation, and an interactive paraphrasing interface. Fully implemented in Python with Hugging Face Transformers.
Transformers • Grammar Correction • Semantic Similarity • Evaluation Metrics
<p align="center">
<img src="https://img.shields.io/badge/Python-3.10-blue" />
<img src="https://img.shields.io/badge/Transformers-T5%20Small-green" />
<img src="https://img.shields.io/badge/Sentence--BERT-MiniLM--L6--v2-orange" />
<img src="https://img.shields.io/badge/Colab-Compatible-yellow" />
<img src="https://img.shields.io/badge/Status-Active-success" />
</p>

## Overview
This project implements a complete AI-powered paraphrasing pipeline using:

T5-small for paraphrase generation

LanguageTool for grammar correction

Sentence-BERT (MiniLM-L6-v2) for semantic similarity

BLEU & ROUGE for evaluation metrics

It rewrites text while preserving meaning, improving clarity, and ensuring linguistic correctness. Ideal for NLP learners, students, and content creators.

## Features
✔️ Transformer-based paraphrasing (T5-small)

✔️ Grammar correction using LanguageTool

✔️ Semantic similarity scoring with Sentence-BERT

✔️ BLEU & ROUGE evaluation metrics

✔️ Interactive paraphrasing mode

✔️ Clean, modular Python functions

✔️ Fully runnable in Google Colab

## Tech Stack
Python

Hugging Face Transformers

PyTorch

Sentence-Transformers

LanguageTool

SacreBLEU

ROUGE Score

## Installation
Run this in Google Colab:
!pip install -q transformers sentencepiece language-tool-python sacrebleu rouge-score sentence-transformers

## Model Loading
from transformers import T5Tokenizer, T5ForConditionalGeneration
tokenizer = T5Tokenizer.from_pretrained("t5-small")
model = T5ForConditionalGeneration.from_pretrained("t5-small")

Grammar checker:
import language_tool_python
grammar_tool = language_tool_python.LanguageTool('en-US')

Semantic similarity:
from sentence_transformers import SentenceTransformer
sim_model = SentenceTransformer('all-MiniLM-L6-v2')


## Evaluation Metrics
BLEU score

ROUGE-1, ROUGE-2, ROUGE-L

Average semantic similarity

## Project Structure
├── AI-powered-paraphrasing-tool.ipynb   # Main notebook
├── README.md


