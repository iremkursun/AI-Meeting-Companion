# AI Meeting Companion

An AI-powered meeting assistant that transcribes business meeting audio with **OpenAI Whisper**, summarizes the discussion and extracts key points using **IBM watsonx.ai** LLMs, and serves everything through a simple **Hugging Face Gradio** web interface.

> Built as part of the IBM Skills Network lab **"Business AI Meeting Companion"**.

---


## Features

- **Speech-to-Text:** Converts meeting or lecture recordings into accurate text using OpenAI Whisper (`openai/whisper-tiny.en`).
- **Summarization & Key Points:** Uses IBM watsonx.ai large language models to produce concise summaries and highlight key decisions.
- **Web Interface:** Upload an audio file and view the results in a user-friendly Gradio app.

---
## Demo

Upload a meeting recording and the app returns the transcript along with key points extracted by the LLM:<img width="613" height="487" alt="AI Meeting Companion" src="https://github.com/user-attachments/assets/5f688ce3-4772-4a8b-af69-146df4a26d0b" />

---
## Tech Stack

| Component        | Technology                          |
|------------------|-------------------------------------|
| Language         | Python 3                            |
| Speech-to-Text   | OpenAI Whisper (Hugging Face Transformers) |
| LLM              | IBM watsonx.ai                      |
| UI               | Gradio                              |
| Deep Learning    | PyTorch                             |

---

## Project Structure

```
AI-Meeting-Companion/
├── download_audio.py       # Downloads the sample audio file
├── simple_speech2text.py   # Transcribes audio to text with Whisper
├── hello.py                # Simple Gradio demo app
├── speech2text_app.py      # Gradio app for audio transcription
├── downloaded_audio.mp3    # Sample audio file
└── README.md
```

---

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/iremkursun/AI-Meeting-Companion.git
   cd AI-Meeting-Companion
   ```

2. **Create and activate a virtual environment**
   ```bash
   python3 -m venv my_env
   source my_env/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install torch transformers gradio requests
   ```

---

## Usage

### 1. Download the sample audio
```bash
python3 download_audio.py
```

### 2. Transcribe audio in the terminal
```bash
python3 simple_speech2text.py
```

### 3. Launch the Gradio app
```bash
python3 speech2text_app.py
```
Then open **http://localhost:7860** in your browser, upload an audio file, and see the transcription.

---

## Learning Objectives

- Generate text with a model from the Hugging Face Hub and understand key parameters that influence the output.
- Use OpenAI Whisper to convert recordings into text.
- Use IBM watsonx.ai to summarize transcripts and extract key points.
- Build an intuitive user interface with Hugging Face Gradio.

---

## License

Lab content is licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0).

## Author

**İrem Kurşun** – [GitHub](https://github.com/iremkursun)
