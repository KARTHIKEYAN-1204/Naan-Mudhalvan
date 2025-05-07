📝 Script Description

This Python script performs the following steps:

    Listens to spoken input from the microphone.

    Uses Google's Speech Recognition API to convert spoken words into text.

    Translates the recognized text into a user-specified target language using the Google Translate API.

    Prints both the original and translated text.

It’s useful for voice-based translation tasks or creating voice-assisted apps.
📦 Required Python Packages

To run the script successfully, you need the following packages:
Package	Purpose	Install Command
speechrecognition	Recognize speech from microphone/audio	pip install SpeechRecognition
pyaudio	Interface with the microphone	pip install pyaudio (see note below)
googletrans==4.0.0-rc1	Translate text using Google Translate	pip install googletrans==4.0.0-rc1

    ⚠️ Note: PyAudio may fail to install via pip alone due to missing system dependencies. Install system packages first:

🔧 For Debian/Ubuntu:

sudo apt install portaudio19-dev python3-pyaudio

Then install PyAudio via pip:

pip install pyaudio

✅ Optional: Full Requirements List for requirements.txt

If you want to put this in a requirements.txt file:

SpeechRecognition
pyaudio
googletrans==4.0.0-rc1
