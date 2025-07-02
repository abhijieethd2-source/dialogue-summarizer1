# Real-Time Multilingual Speech Recognition and Speaker Diarization System

This project integrates OpenAI's Whisper ASR, MarbleNet Voice Activity Detection (VAD), TitaNet speaker embeddings, and CTC-based forced alignment to build a real-time system for transcribing multilingual speech with accurate speaker attribution.

## Features
- Real-time transcription with Whisper ASR
- Voice activity detection using MarbleNet
- Speaker diarization with TitaNet embeddings
- Word-level forced alignment for precise timestamps
- Multilingual support (English, Hindi, Telugu, etc.)
- RESTful API deployment with FastAPI and Docker for scalable use

## Architecture Overview
1. **Audio Input:** Accepts live audio stream or prerecorded files
2. **VAD:** MarbleNet detects speech segments
3. **ASR:** Whisper transcribes speech segments into text
4. **Speaker Embeddings:** TitaNet extracts speaker features for diarization
5. **Alignment:** Forced alignment maps text to audio timestamps
6. **Output:** Time-stamped transcripts labeled by speaker

## Setup Instructions

### Prerequisites
- Python 3.8+
- Docker (optional but recommended)
- ffmpeg (for audio processing)

### Installation
```bash
git clone <your-repo-url>
cd <your-repo-folder>
pip install -r requirements.txt
