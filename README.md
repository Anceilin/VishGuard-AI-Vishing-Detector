# VishGuard - AI Vishing Detector

VishGuard is a web application designed to analyze audio recordings and identify potential voice-phishing (vishing) risks.

## Features

- Upload audio recordings in WAV or MP3 format.
- Analyze potential voice-phishing risks.
- Generate transcripts from audio.
- Extract suspicious keywords.
- Detect the language of the transcript.
- Report and manage suspicious phone numbers.
- View results through a Streamlit interface.

## Tech Stack

- **Frontend:** Streamlit
- **Backend API:** FastAPI, Uvicorn
- **Language:** Python
- **Machine Learning:** scikit-learn, audio feature extraction
- **Speech-to-Text:** OpenAI Whisper
- **Database:** SQLite

## Prerequisites

- Python 3.10 or a compatible version
- pip

## Installation

Clone the repository, then open its directory in your terminal.

Install the dependencies:

```bash
pip install -r requirements.txt
```

## Run the Application

Start the FastAPI backend in the first terminal:

```bash
python -m uvicorn api:app --reload --host 127.0.0.1 --port 8000
```

Start the Streamlit interface in a second terminal:

```bash
python -m streamlit run app.py
```

Open the local Streamlit URL shown in the terminal, usually `http://localhost:8501`.

The backend API documentation is usually available at `http://127.0.0.1:8000/docs`.

## Important Notes

- Audio analysis results are predictions and should not be treated as definitive proof of fraud.
- Detection quality depends on the model, audio quality, and input data.
- Keep private recordings, datasets, database files, and credentials out of public repositories.
- Some features may require additional setup depending on the installed dependencies.

## Project Status

Developed as an AI and full-stack project to explore voice analysis, speech processing, and potential vishing-risk detection.
