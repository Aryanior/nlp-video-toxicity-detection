# Video Toxicity Detector

An end-to-end NLP application that detects toxic speech in videos by extracting audio, converting speech to text, preprocessing the transcript, and classifying toxicity using a trained LightGBM model. The project features an interactive Gradio interface for real-time analysis.

---

## Overview

This project automates the process of identifying toxic speech in video content. It extracts audio from uploaded videos, transcribes the speech into text, applies Natural Language Processing (NLP) techniques for text preprocessing, and predicts whether the content is toxic along with its toxicity categories.

This solution can be useful for:
- Social media content moderation
- Video content screening
- Educational demonstrations of NLP pipelines
- Speech-based toxicity analysis

---

##  Features

- Upload video files for analysis
- Automatic audio extraction from videos
- Speech-to-Text transcription
- Text preprocessing using NLTK
- TF-IDF feature extraction
- Toxicity prediction using a trained LightGBM model
- Detects multiple toxicity categories
- Interactive Gradio web interface
- Real-time prediction results

---

## Tech Stack

- Python
- Scikit-learn
- LightGBM
- NLTK
- SpeechRecognition
- MoviePy
- Gradio
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## How It Works

1. Upload a video through the Gradio interface.
2. Audio is extracted from the uploaded video.
3. The extracted audio is converted into text using Google's Speech Recognition API.
4. The transcript is cleaned and preprocessed using NLP techniques:
   - Lowercasing
   - Contraction expansion
   - Tokenization
   - Stopword removal
   - Stemming
5. The processed text is transformed into TF-IDF features.
6. The trained LightGBM classifier predicts the toxicity probabilities.
7. The application displays:
   - Video transcript
   - Toxicity prediction
   - Toxicity categories detected

---

## Project Structure

```
video-toxicity-detector/
│
├── app.py
├── model.pkl
├── vectorizer.pkl
├── requirements.txt
├── README.md
└── screenshots/
```

---

##Installation

Clone the repository

```bash
git clone https://github.com/your-username/video-toxicity-detector.git
```

Move into the project directory

```bash
cd video-toxicity-detector
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the application

```bash
python app.py
```

---

## Demo

Upload a video file and the application will return:

- Speech Transcript
- Toxicity Classification
- Toxicity Categories (if detected)

*(Add screenshots here after uploading them.)*

---

## Model Pipeline

Video Input
↓
Audio Extraction (MoviePy)
↓
Speech Recognition
↓
Text Preprocessing (NLTK)
↓
TF-IDF Vectorization
↓
LightGBM Classifier
↓
Toxicity Prediction

---

## Libraries Used

- scikit-learn
- LightGBM
- SpeechRecognition
- MoviePy
- Gradio
- Pandas
- NumPy
- NLTK
- Matplotlib
- Seaborn

---

## Future Improvements

- Support multiple languages
- Real-time microphone analysis
- Timestamp-based toxicity detection
- Confidence score visualization
- Speaker diarization
- Deploy using Docker
- Cloud deployment on Hugging Face Spaces or Render

---

## Author

**Aryan Mathuriya**

Artificial Intelligence & Data Science Student

Interested in Machine Learning, NLP, Data Science, and AI Applications.

---

## ⭐ If you found this project useful, consider giving it a star!
