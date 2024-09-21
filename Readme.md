# ST-Transcriber-DeepSpeech

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Troubleshooting](#troubleshooting)

## Overview

ST-Transcriber is a real-time speech-to-text application built with Streamlit and DeepSpeech. It allows users to convert spoken audio into written text, providing an easy-to-use interface for transcribing audio files.

## Features

- Real-time speech recognition
- Support for both audio-only and audio-with-video input
- Integration with DeepSpeech for accurate transcription
- Interactive web interface using Streamlit
- Optional video conferencing capabilities

## Requirements

- Python 3.7+
- Streamlit
- DeepSpeech
- Pydub
- Av
- Twilio (for optional video conferencing)

## Installation

1. Clone the repository:
clone https://github.com/NafisRayan/ST-Transcriber-DeepSpeech


2. Set up the virtual environment:
python -m venv myenv source myenv/bin/activate # On Windows, use myenv\Scripts\activate


3. Install dependencies:
pip install -r requirements.txt


## Usage

1. Run the application:
streamlit run app.py


2. Open the URL provided in your web browser (usually http://localhost:8501).

3. Choose between "Sound only" or "With video" mode using the selectbox.

4. Speak into your microphone or participate in a video call.

5. The transcribed text will appear on the screen in real-time.

## Configuration

To enable Twilio credentials for video conferencing:

1. Set the following environment variables:
export TWILIO_ACCOUNT_SID=your_account_sid export TWILIO_AUTH_TOKEN=your_auth_token


## Troubleshooting

- If Twilio credentials are not set, the app will fall back to using Google's STUN server.
- Ensure you have the necessary permissions to access your microphone and camera.
- If you encounter issues with ffmpeg, try installing it separately.
- For Windows users, some network-related warnings may appear but should not affect functionality.

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues on the GitHub repository.