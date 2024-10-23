# Social-Bot-Detection

## Research Problem
The problem involves detecting automated bot accounts on Twitter (now X) that spread misinformation and manipulate public opinion. This is significant because:

* Bot accounts can artificially amplify certain messages
* They can manipulate trending topics and discussions
* They potentially influence user behavior and opinions

## Research Gap
This project addresses these key gaps:

* Existing solutions often focus on single features (like text only or metadata only)
* Previous approaches may not handle real-time detection effectively
* Many current solutions don't combine both text and numerical features for classification

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
