# Text-to-Speech

# Phonetics Transcription Tool

## Overview
This Phonetics Transcription Tool converts input text into International Phonetic Alphabet (IPA) transcription, provides phoneme breakdowns, and generates audio pronunciation where possible. The tool supports multiple languages and scripts using `pronouncing`, `epitran`, and `gTTS` for text-to-speech conversion.

## Features
- Converts text into IPA transcription.
- Provides phoneme breakdowns with descriptions.
- Supports multiple languages and scripts.
- Generates audio pronunciation using Google Text-to-Speech (`gTTS`).
- Interactive user interface built with `Gradio`.

## Installation
Before running the project, install the required dependencies:

```bash
pip install pronouncing epitran gtts gradio IPython
```

## Usage
1. Run the script to launch the Gradio interface.
2. Enter the text you want to transcribe.
3. Select the language/script pair from the dropdown menu.
4. Click the "Process" button to generate IPA transcription and phoneme breakdown.
5. If audio is available for the selected language, playback will be provided.

## Project Structure
- `transcribe_to_ipa(text, language)`: Converts input text to IPA transcription.
- `arpabet_to_ipa(arpabet)`: Maps ARPAbet phonemes to IPA symbols.
- `explain_phonemes(ipa)`: Breaks down IPA transcription into phonetic descriptions.
- `process_input(text, language)`: Handles the transcription process and generates audio output.
- `Gradio Interface`: Provides an interactive UI for users.

## Supported Languages
This tool supports a wide range of languages and scripts, including:
- English (en-US, eng-Latn)
- Spanish (spa-Latn)
- French (fra-Latn)
- German (deu-Latn)
- Chinese (cmn-Hans, cmn-Hant)
- Japanese (jpn-Hrgn, jpn-Ktkn)
- Korean (kor-Hang)
- And many more...

## Running the Tool
To start the application, run:

```bash
python Text_to_Speech.py
```

Then, open the provided Gradio URL in your web browser.

## Troubleshooting
- If `gTTS` fails to generate audio, ensure you have an active internet connection.
- Some languages may not be supported by `epitran`, leading to transcription errors.
- Ensure all dependencies are installed correctly before running the script.

## License
This project is open-source and available for personal and educational use. Modify and distribute as needed!

## Author
Developed by Afzal y. Feel free to contribute or suggest improvements!

