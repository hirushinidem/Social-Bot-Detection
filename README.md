# 🤖 Social-Bot-Detection

A hybrid deep learning approach for detecting automated bot accounts on Twitter using LSTM and dense neural networks.

## 📝 Introduction
Social media platforms like Twitter face significant challenges from automated bot accounts that can:
- 🔄 Manipulate public opinion
- ❌ Spread misinformation
- 🔨 Disrupt genuine user interactions

## 🎯 Problem Statement
- 📈 Growing presence of automated bot accounts
- 🔍 Difficulty in distinguishing between human and bot content
- ⚡ Need for accurate, real-time detection mechanisms

## ⚠️ Current Limitations
Existing solutions often rely on:
- 📊 Single feature analysis
- 🔢 Basic classification methods
- 📉 Limited feature extraction

## 🛠️ Methodology

### Data Processing
#### Text Processing
- 📚 Tokenization of tweet text
- 📏 Padding sequences to uniform length
- 🧹 Text cleaning (removing digits, punctuation)

#### Feature Extraction
- @ User mentions count
- # Hashtag count
- 🏢 Organization and Person entity percentages

### Model Architecture
```python
model = {
    "Text Branch": {
        "Embedding Layer": "Word embeddings",
        "LSTM Layer": "Sequence processing"
    },
    "Numeric Branch": {
        "Dense Layer": "Numeric feature processing"
    },
    "Combined": {
        "Concatenation": "Feature fusion",
        "Dense Layers": "With dropout",
        "Output": "Sigmoid activation"
    }
}
