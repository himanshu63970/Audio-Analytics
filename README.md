Here’s a README file for your GitHub repository. This will help others understand how to use your application and what it does:

---

# Audio Sentiment Analysis Dashboard

## Overview

The **Audio Sentiment Analysis Dashboard** is a GUI application developed using Python's Tkinter library. It provides a platform for analyzing audio files and recordings for sentiment analysis. The application utilizes speech recognition to transcribe audio and a sentiment analysis pipeline from the Hugging Face Transformers library to determine the sentiment of the transcribed text. It also supports language detection and visualizes sentiment results using matplotlib.

## Features

- **Upload Audio**: Select and analyze audio files in formats like WAV, MP3, and FLAC.
- **Record Audio**: Record audio directly from the microphone and analyze the sentiment.
- **Detect Language**: Identify the language of the transcribed text.
- **Clear Text**: Reset the display area and remove the plot.
- **Help**: Provides information on how to use the application.
- **Exit**: Close the application.

## Installation

### Prerequisites

Ensure you have Python installed (Python 3.7 or later). You will also need to install the following Python libraries:

- `tkinter`: Standard GUI library (included with Python)
- `pillow`: For image processing
- `speech_recognition`: For audio transcription
- `transformers`: For sentiment analysis
- `torch`: Required by transformers
- `matplotlib`: For plotting
- `numpy`: For numerical operations
- `langdetect`: For language detection

You can install the necessary libraries using pip:

```bash
pip install pillow speech_recognition transformers torch matplotlib numpy langdetect
```

## Usage

1. **Run the Application**: Execute the script `app.py` to start the application.

    ```bash
    python app.py
    ```

2. **Upload Audio**:
   - Click on the "Upload Audio" button to select and analyze an audio file.
   - Supported formats: WAV, MP3, FLAC.

3. **Record Audio**:
   - Click on the "Record Audio" button to record audio from your microphone. The recording will last for 10 seconds.

4. **Detect Language**:
   - Click on the "Detect Language" button to identify the language of the transcribed text.

5. **Clear Text**:
   - Click on the "Clear Text" button to reset the display area and remove the plot.

6. **Help**:
   - Click on the "Help" button to view instructions on how to use the application.

7. **Exit**:
   - Click on the "Exit" button to close the application.

## Code Overview

- **`transcribe_audio(audio_path)`**: Transcribes audio files to text using the `speech_recognition` library.
- **`analyze_sentiment(text)`**: Analyzes the sentiment of the transcribed text using the `transformers` library.
- **`plot_sentiment(sentiments)`**: Plots sentiment analysis results using `matplotlib`.
- **`highlight_sentiments(text)`**: Highlights words in the text based on their sentiment.
- **`get_repeated_words(text)`**: Identifies repeated words in the transcribed text.
- **`get_sentiment_explanation(sentiment, positive_words, negative_words)`**: Provides an explanation for the sentiment classification.

## Contributing

Feel free to contribute to this project by submitting issues or pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to adjust any sections to better fit your specific project details or preferences!
