# 🤖 Social-Bot-Detection

A hybrid deep learning approach for detecting automated bot accounts on Twitter using LSTM and dense neural networks.

## 📝 Introduction
Social media platforms like Twitter face significant challenges from automated bot accounts that can:
- Manipulate public opinion
- Spread misinformation
- Disrupt genuine user interactions

## 🎯 Problem Statement
- Growing presence of automated bot accounts
- Difficulty in distinguishing between human and bot content
- Need for accurate, real-time detection mechanisms

## ⚠️ Current Limitations
Existing solutions often rely on:
- Single feature analysis
- Basic classification methods
- Limited feature extraction

## 🛠️ Methodology
### Model Architecture
* Text Input Branch:
   - Embedding layer
   - LSTM layer
* Numerical Input Branch:
   - Dense layer for numeric features
* Combined Architecture:
   - Concatenation of both branches
   - Multiple dense layers with dropout
  - Final sigmoid output layer
### Training Process
* Used Adam optimizer
* Binary cross-entropy loss
* Early stopping to prevent overfitting
* Validation split of 20%

The model achieved approximately 97% accuracy on the test set, demonstrating effective bot detection capabilities. 

