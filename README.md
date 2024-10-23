# Social-Bot-Detection

## Introduction
Social media platforms like Twitter face significant challenges from automated bot accounts. These bots can manipulate public opinion, spread misinformation, and disrupt genuine user interactions.

## Problem Statement

* Growing presence of automated bot accounts on social media
* Difficulty in distinguishing between human and bot-generated content
* Need for accurate, real-time bot detection mechanisms

## Current Limitations:
The code implementation addresses these key limitations in existing solutions:
* Current systems often use:
- Single feature analysis (only text OR metadata)
- Basic classification methods
- Limited feature extraction

## Methodology
The project uses a hybrid neural network approach combining:

### Data Processing

#### Text processing
- Tokenization of tweet text
- Padding sequences to uniform length
- Cleaning text (removing digits, punctuation, etc.)

#### Feature extraction
- User mentions count
- Hashtag count
- Organization and Person entity percentages

### Model Architecture

- Text Input Branch:
  - Embedding layer
  - LSTM layer
  
- Numerical Input Branch:
  - Dense layer for numeric features
  
- Combined Architecture:
  - Concatenation of both branches
  - Multiple dense layers with dropout
  - Final sigmoid output layer

### Training Process

- Used Adam optimizer
- Binary cross-entropy loss
- Early stopping to prevent overfitting
- Validation split of 20%
  
The model achieved approximately 97% accuracy on the test set, demonstrating effective bot detection capabilities.
