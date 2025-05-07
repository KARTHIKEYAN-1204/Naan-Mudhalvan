📝 Description

This Python script allows users to:

    Speak a search query through the microphone.

    Convert speech to text using Google's Speech Recognition API.

    Perform a web search using the googlesearch module.

    Read the query and response back to the user using text-to-speech (pyttsx3).

It's essentially a voice-activated mini search assistant.
📦 Required Python Packages
Package	Purpose	Install Command
SpeechRecognition	Captures and processes microphone input	pip install SpeechRecognition
PyAudio	Interface to the microphone (needed by SR)	See PyAudio Setup below
pyttsx3	Text-to-speech engine (offline TTS)	pip install pyttsx3
googlesearch-python	Perform Google search queries	pip install googlesearch-python

    ⚠️ Important: googlesearch is not officially maintained by Google and may occasionally break or rate-limit. Use responsibly.

🔧 PyAudio Setup (for Linux)

PyAudio depends on the PortAudio system package. Install it before installing PyAudio via pip:

sudo apt update
sudo apt install portaudio19-dev python3-pyaudio
pip install pyaudio

If you're using UserLAnd or a virtualized terminal, PyAudio may fail due to hardware/microphone access limitations.
✅ requirements.txt

If you want to save the required libraries in a requirements.txt file:

SpeechRecognition
pyaudio
pyttsx3
googlesearch-python

🛠️ Troubleshooting

    Microphone not working? Make sure your device has mic access and try listing audio input devices with:

arecord -l

Speech not recognized? Check internet connection and ambient noise levels.

Jack/ALSA errors? These are common in environments like WSL or UserLAnd and may not affect functionality.
