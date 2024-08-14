## Overview

This project automates the creation of a specialized speech-to-text dataset from YouTube videos, specifically designed for fine-tuning Text-to-Speech (TTS) models and voice cloning. The code extracts and processes audio from videos, generates accurate transcriptions, and organizes the data into a structured format suitable for training TTS systems and creating personalized voice models.

## Features

- **Automated Audio Extraction:** Download and extract high-quality audio from YouTube videos with ease.
- **Precise Speech-to-Text Transcription:** Utilize advanced speech recognition models to transcribe audio into text with high accuracy, ensuring the dataset is robust for TTS and voice cloning tasks.
- **Dataset Structuring for TTS:** Organize transcriptions and corresponding audio files into a format that is optimized for TTS model fine-tuning, including appropriate training and validation splits.
- **Voice Cloning Capabilities:** Enable the creation of personalized voice models by generating datasets from specific speakers' audio, ideal for voice cloning applications.
- **Phoneme Conversion:** Optionally convert transcriptions into phonemes to enhance linguistic features in TTS models.
- **Customizable Workflow:** Adjust token lengths, buffer times, and other parameters to tailor the dataset creation process to your specific needs.

## Usage

1. **Setup:** Install the required dependencies and configure your environment for dataset creation.
2. **Execution:** Run the provided scripts to extract audio, transcribe speech, and generate a dataset optimized for TTS fine-tuning and voice cloning.
3. **Output:** The final output includes well-organized audio files, transcriptions, and optional phonemized text files, ready for use in fine-tuning TTS models or creating custom voice clones.

## Requirements

- Python 3.7+
- `pytube` for downloading YouTube videos
- `pydub` for processing audio files
- `whisper` or `espeak-ng` for speech recognition
- `phonemizer` for phoneme conversion (optional)
- TTS models and frameworks such as Tacotron, FastSpeech, or WaveNet (for fine-tuning)

## How It Works

1. **Audio Extraction:** The script downloads YouTube videos and extracts audio in `.wav` format, preserving the quality needed for TTS and voice cloning tasks.
2. **Transcription:** The extracted audio is transcribed using cutting-edge speech-to-text models, ensuring the text is highly accurate for TTS model training.
3. **Dataset Structuring:** Transcriptions are paired with their corresponding audio files and structured into training and validation sets, ready for TTS fine-tuning or voice cloning.
4. **Phonemization (Optional):** Transcriptions are converted into phonemes, providing an additional layer of linguistic data for enhancing TTS models.

## Applications

- **Fine-Tuning Text-to-Speech (TTS) Models:** Use the generated dataset to fine-tune existing TTS models for more natural and expressive speech synthesis.
- **Voice Cloning:** Create personalized voice models by generating datasets from specific speakers, enabling voice cloning for applications such as virtual assistants, personalized audio content, and more.
