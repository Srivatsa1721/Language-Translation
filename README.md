
# Voice-to-Text Translation Application

This Python application collects voice input, recognizes the spoken text, determines the language, translates it into a target language, and outputs an audio file in the translated language.

## Features

- **Voice Input**: Captures your voice input through the microphone.
- **Speech Recognition**: Recognizes the spoken text using Google Speech Recognition.
- **Language Detection**: Automatically detects the language of the recognized text.
- **Translation**: Translates the recognized text into a target language specified by the user.
- **Text-to-Speech**: Converts the translated text into an audio file using Google Text-to-Speech (gTTS).
- **Audio Playback**: Plays the translated audio file based on your system's OS (Windows, macOS, or Linux).

## Prerequisites

Ensure you have the following installed:

- **Python 3.7 or higher**

Required Python libraries (install via pip):

- `speech_recognition`
- `googletrans==4.0.0-rc1`
- `gtts`

## Installation

1. **Clone this repository**:
   ```bash
   git clone https://github.com/your-repository-name/voice-to-text-translation.git

2. **Set up a virtual environment(recommended)**:

- For Windows:
   ```bash
   python -m venv venv
   venv\Scripts\activate

- For macOS/Linux:
   ```bash
   python -m venv venv
   source venv/bin/activate

3. **Install the required libraries by running**:
   ```bash
   pip install -r requirements.txt

4. **Ensure your microphone is connected and working properly.**

## Usage

1. **Run the script**:

Open a terminal or command prompt and run the following command:
   
   ```python app.py```
   
2. **Select the target language when prompted. You can choose from the following languages**:

- French (fr)
- Spanish (es)
- German (de)
- Portuguese (pt)
- Hindi (hi)
- Telugu (te)
- Tamil (ta)
- Malayalam (ml)

3. **Speak into the microphone when instructed. The application will-**:

- Recognize your speech.
- Detect the language of the recognized text.
- Translate the text into the specified target language.
- Save the translated text as an audio file in the outputs/ folder.

4. **Audio Playback**: The translated audio will automatically play after the translation. The playback command will vary depending on your operating system:

- Windows: start
- macOS: open
- Linux: xdg-open

## Supported Languages

The application currently supports the following languages for translation:

- French (fr)
- Spanish (es)
- German (de)
- Portuguese (pt)
- Hindi (hi)
- Telugu (te)
- Tamil (ta)
- Malayalam (ml)

## File Structure

Here’s the structure of the project directory:

```sql
voice-to-text-translation/
|-- app.py              # Main application script
|-- requirements.txt    # Required libraries
|-- outputs/            # Directory where translated audio files are saved
```

## Requirements File

Create a requirements.txt file with the following content:

```makefile
speech_recognition
googletrans==4.0.0-rc1
gtts
```

## Notes

Occasionally, the googletrans library may experience issues with translations. If translation fails, check your internet connection or try again later.
The outputs folder will be created automatically if it doesn't exist. This folder will store all the generated translated audio files.
