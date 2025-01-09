This project consists of three main components: an emotion detection function, a unit test for validation, and a Flask-based server for hosting the application. Here's a summary:

Emotion Detector:
The emotion_detector function uses the requests library to send text to a Watson NLP API for emotion analysis.
It processes the API's JSON response to extract emotion scores (e.g., anger, joy) and identifies the dominant emotion.
The function returns a dictionary with emotion scores and the dominant emotion.
Unit Testing:
The TestEmotionDetection class tests the emotion_detector function with predefined text inputs and validates if the dominant emotion matches expectations using the unittest framework.
This ensures the function's correctness.
Flask Server:
The Flask app provides an endpoint /emotionDetector to analyze emotions from a given text query parameter.
It uses the emotion_detector function to process input and returns a formatted response or error messages.
An additional / route renders a web interface for the application.
