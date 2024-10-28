# Twitter Bot Detection

## Overview
A deep learning component that detects Twitter bots using a hybrid approach combining text analysis and numerical features. Part of a larger system for detecting social media misinformation.

## Features
- Hybrid neural network architecture combining LSTM and Dense layers
- Text and numerical feature processing 
- Trained on synthetic and real Twitter data
- Focus on Sri Lankan Twitter context

## Model Architecture

- Text Processing: LSTM layer for tweet content analysis
- Numerical Processing: Dense layers for user behavior metrics
- Combined through concatenation layer
- Binary classification output (bot/not bot)
