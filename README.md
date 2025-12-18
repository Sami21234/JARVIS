# JARVIS – Voice-Activated Virtual Assistant 🎙️🤖

## 📌 Project Overview
**Jarvis** is a voice-activated virtual assistant developed in Python.  
It listens for voice commands, responds using speech, performs web-based and system tasks, fetches news, plays music, and answers user queries using an AI language model.

The assistant is activated using a **wake word: “Jarvis”**, similar to Alexa or Google Assistant.

---

## ✨ Features

### 🎤 Voice Recognition
- Uses the `speech_recognition` library.
- Continuously listens for the wake word **“Jarvis”**.
- Converts spoken commands into text.

### 🔊 Text-to-Speech
- Converts responses into speech using **Windows SAPI (pywin32)**.
- Provides natural voice feedback for all actions.

### 🌐 Web Browsing
- Opens popular websites using voice commands:
  - Google
  - Facebook
  - YouTube
  - LinkedIn

### 🎵 Music Playback
- Plays music using a custom `musicLibrary` module.
- Opens song links in the web browser.

### 📰 News Fetching
- Fetches latest news headlines using **NewsAPI**.
- Reads out top headlines using text-to-speech.

### 🤖 AI Integration
- Handles complex or unknown commands using an AI language model.
- Acts as a general-purpose assistant for questions and conversations.
- Provides brief and helpful responses.

### 🖥️ System Operations
- Opens local applications such as:
  - Calculator
  - VS Code
  - File Explorer
  - WhatsApp (if installed)

---

## 🔄 Workflow

1. **Initialization**
   - Jarvis starts and greets the user with  
     **“Initializing Jarvis…”**

2. **Wake Word Detection**
   - Listens continuously for the wake word **“Jarvis”**.

3. **Activation**
   - Upon detecting the wake word, Jarvis replies with **“Ya”**.

4. **Command Processing**
   - Listens for the user’s command.
   - Determines whether the command is:
     - A fixed task (open apps, play music, fetch news)
     - Or an AI-based query

5. **Execution**
   - Performs the requested action.
   - Uses AI responses if no predefined command matches.

6. **Speech Output**
   - Responds using text-to-speech.

---

## 🛠️ Libraries Used

- `speech_recognition` – Voice input recognition  
- `webbrowser` – Open websites via commands  
- `pywin32 (win32com.client)` – Text-to-speech using Windows SAPI  
- `musicLibrary` – Custom module for music playback  
- `requests` – Fetch news from NewsAPI  
- `os` – Open system applications  

---

## 🖥️ System Requirements

- Windows OS  
- Python 3.9+  
- Microphone  
- Internet connection (for news & AI responses)

---

## 🚀 How to Run the Project

1. Clone or download the repository.
2. Install required libraries:
   ```bash
   pip install speechrecognition requests pywin32 groq
3. Add your API key in config.py.
4. Run the program:
   ```bash
   python main.py
5. Say “Jarvis” to activate.

---

## 👨‍💻 Author

Developed to enhance the python skills to demonstrate:

- Voice recognition
- System automation
- AI integration
- Python programming skills

## ✅ Future Enhancements

- GUI interface (Tkinter / PyQt)
- Offline wake-word detection
- Intent classification using ML
- Plugin-based command system
- Cross-platform support
