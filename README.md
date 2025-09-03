# Bird Sound Matcher

## Overview
The Bird Sound Matcher is a Python application designed to record audio, convert it into spectrograms, and find similar bird sounds using cosine similarity. The application retrieves audio files and their corresponding spectrograms from Google Drive, processes the audio input, and displays the top 5 matches based on similarity scores.

## Features
- Record audio from the microphone.
- Convert recorded audio into spectrograms.
- Retrieve bird sound files and spectrograms from Google Drive.
- Compute cosine similarity to find the most similar bird sounds.
- Display the names of the top 5 matches.

## Project Structure
```
bird-sound-matcher
├── src
│   ├── main.py                # Entry point of the application
│   ├── audio
│   │   ├── __init__.py        # Marks audio directory as a package
│   │   ├── recorder.py         # Handles audio recording
│   │   ├── spectrogram.py      # Converts audio to spectrogram
│   ├── data
│   │   ├── __init__.py        # Marks data directory as a package
│   │   ├── google_drive.py     # Accesses audio files from Google Drive
│   ├── similarity
│   │   ├── __init__.py        # Marks similarity directory as a package
│   │   ├── matcher.py          # Computes similarity scores
│   └── utils
│       └── __init__.py        # Marks utils directory as a package
├── requirements.txt            # Lists project dependencies
└── README.md                   # Documentation for the project
```

## Setup Instructions
1. Clone the repository:
   ```
   git clone <repository-url>
   cd bird-sound-matcher
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Set up Google Drive API credentials to access audio files.

## Usage
1. Run the application:
   ```
   python src/main.py
   ```

2. Follow the prompts to record audio and retrieve similar bird sounds.

## Dependencies
- librosa
- pydub
- numpy
- Google Drive API libraries

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any enhancements or bug fixes.

## License
This project is licensed under the MIT License.