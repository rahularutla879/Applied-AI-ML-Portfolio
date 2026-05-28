# Predicting Drug Side Effects using Integrated Molecular Embeddings and Physicochemical Features

## Overview
This project focuses on predicting adverse drug reactions using machine learning. The main idea was to combine molecular structure information with traditional physicochemical drug features to predict possible side effects.

## Problem
Adverse drug reactions are a major issue in drug development and patient safety. Traditional monitoring often happens after drugs are already in use, so this project explores whether machine learning can help predict potential side effects earlier using available drug data.

## Approach
The project combines two types of drug representations:

- ChemBERTa molecular embeddings generated from SMILES strings
- Physicochemical features such as molecular weight, LogP, H-bond donors, H-bond acceptors, polar surface area, and related chemical properties

These features were used to train a multi-label classification model that predicts the presence or absence of different side effects.

## Dataset
The project used publicly available drug and side effect data from sources such as SIDER and DrugBank, along with curated SMILES strings and physicochemical properties.

## Tools and Methods
- Python
- PyTorch
- Hugging Face Transformers
- ChemBERTa
- scikit-learn
- Multi-label classification
- MLP neural network
- SHAP / explainable AI

## Key Results
The project found that combining ChemBERTa molecular embeddings with physicochemical features improved prediction performance compared to using either feature type alone.

## Key Learning
This project showed how chemical language models can be used to represent molecular structure and how those embeddings can be combined with traditional drug features for healthcare prediction tasks.

## Files
- `Predicting Drug Side Effects using.pdf` — Full project report
