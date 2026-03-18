# Image Caption Generator
## Project Overview
This project implements a multimodal deep learning system capable of generating descriptive textual captions for both static images and dynamic video sequences.

## Technical Architecture
The system utilizes an Encoder-Decoder framework to translate visual data into natural language:

### 1. Visual Feature Extraction (Encoder)
CNN Integration: Uses a pre-trained Convolutional Neural Network (e.g., InceptionV3 or VGG16) to extract high-level feature vectors from input frames.

Dimensionality Reduction: Processes raw pixel data into a dense representation that captures the spatial context of the scene.

### 2. Sequence Generation (Decoder)
RNN/LSTM Architecture: An LSTM-based language model predicts the next word in a sequence based on the previous words and the visual features provided by the encoder.

Temporal Processing for Video: For video inputs, the system samples frames and generates captions by maintaining context across the temporal dimension.

## Project Structure & Usage
Inference Engine: Image_Captioning_Testing_Code_Final.ipynb contains the core logic for loading the model and generating captions.

Pre-trained Weights: Utilizes model_final.h5 for optimized performance without the need for additional training.

Input Versatility: Supports standard image formats and video files (accessible via the final cell in the notebook).

## Tech Stack
Frameworks: TensorFlow / Keras

Language: Python

Libraries: NumPy, OpenCV, Matplotlib

Concepts: CNNs, LSTMs, Multimodal Learning, Natural Language Processing (NLP).

Link to pretrained model: https://drive.google.com/file/d/1TuWUMpmQFU7quew6J5JYcTZ0qaPhL-O4/view?usp=sharing
