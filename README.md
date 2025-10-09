# End-to-End-Multilingual-Speech-Processing-Framework-using-Wav2Vec2-and-Neural-Networks
Multilingual Speech Recognition and Translation using Wav2Vec2 and Whisper


🗣️ Multilingual Speech Translator & Language Identifier

This project detects the spoken language from audio, video, or microphone input, transcribes it into text using OpenAI Whisper, translates it into a target Indian language, and generates spoken output using Google Text-to-Speech (gTTS).

It supports 12+ Indian languages, using Wav2Vec2-XLSR for language identification and Whisper for transcription.

🔹 Supported Languages
| Language  | Code |
| --------- | ---- |
| English   | en   |
| Hindi     | hi   |
| Bengali   | bn   |
| Tamil     | ta   |
| Telugu    | te   |
| Kannada   | kn   |
| Malayalam | ml   |
| Marathi   | mr   |
| Gujarati  | gu   |
| Punjabi   | pa   |
| Nepali    | ne   |
| Assamese  | as   |

⚙️ Features

• 🎤 Microphone-based real-time language detection and translation.
• 🎬 Audio extraction from video files and automatic translation.
• 🧠 Wav2Vec2-XLSR for multilingual language identification.
• 💬 OpenAI Whisper for accurate speech-to-text transcription.
• 🌐 Google Translator + gTTS for translation and spoken output.
• 💾 Colab GUI with widgets for easy file upload and recording.
• ⚡ GPU acceleration support for faster processing.

🛠️ Technologies Used

• Python 3
• PyTorch
• HuggingFace Transformers – Wav2Vec2-XLSR for embeddings
• OpenAI Whisper – Speech transcription
• Google Translator (googletrans) – Text translation
• gTTS (Google Text-to-Speech) – Speech synthesis
• MoviePy – Video to audio extraction
• Librosa / SoundFile / SpeechRecognition – Audio processing
• ipywidgets + IPython.display – Interactive Colab GUI

🚀 Getting Started

Clone the repository

git clone https://github.com/<your-username>/multilingual-speech-translator.git
cd multilingual-speech-translator


Create & activate virtual environment

python -m venv .venv
# Windows
.venv\Scripts\activate
# Linux / Mac
source .venv/bin/activate


Install dependencies

pip install -r requirements.txt


Train or Load Pretrained Model (optional)

To train your own language classifier using Wav2Vec2 embeddings, run:

python train_language_classifier.py


Or, place your saved model and scaler files in:

/content/drive/MyDrive/nn/


Run the Translator Interface (Colab or Jupyter)

python multilingual_translator_app.py

🎧 How It Works

Record audio or upload an audio/video file.

The model detects the language using Wav2Vec2 embeddings.

Whisper transcribes the speech into text.

Google Translator converts text into your selected target language.

gTTS speaks out the translated sentence aloud.

⚡ Notes

• For faster transcription, use a GPU-enabled environment.
• Works best on clean speech (background noise may reduce accuracy).
• Supports flexible audio formats: .wav, .mp3, .mp4, .mkv, etc.
• Modify the code to include more Indic or global languages easily.

📌 References

• Wav2Vec2-XLSR Model – HuggingFace

• OpenAI Whisper

• Google Translator (googletrans)

• gTTS (Google Text-to-Speech)

• MoviePy

⭐ Future Improvements

• Add real-time streaming speech translation.
• Add web-based GUI for broader accessibility.
• Integrate noise reduction and voice activity detection.
• Expand support for more regional and global languages.

🌟 Loved this project?

If you enjoyed this project, give it a ⭐ on GitHub!
It helps me stay motivated and continue improving this multilingual AI translator.
