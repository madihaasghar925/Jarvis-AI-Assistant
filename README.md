#  J.A.R.V.I.S.
### Just A Responsive Voice Intelligence System

An offline AI-powered desktop voice assistant built with Python.

JARVIS can understand voice commands, respond using natural speech, open websites, play music, and answer general questions using a locally running Large Language Model (Llama 3 via Ollama).

Unlike traditional voice assistants that depend on cloud APIs, JARVIS performs AI conversations locally, making it faster, privacy-friendly, and completely free to use.

---

#  Features

##  Voice Activation

- Wake word detection ("Jarvis")
- Hands-free interaction
- Continuous microphone listening

---

##  Speech Recognition

- Converts speech into text
- Built using SpeechRecognition
- Google Speech Recognition API

---

##  Local AI Chat

- Powered by Ollama
- Uses Llama 3 locally
- No OpenAI API required
- Offline AI conversations

---

##  Conversation Memory

JARVIS remembers previous conversation within the current session.

Instead of answering each question independently, it sends the conversation history to the LLM, enabling context-aware responses.

---

##  Text-to-Speech

- Natural voice responses
- Powered by pyttsx3
- Completely offline

---

##  Browser Automation

Open websites using voice commands.

Examples:

- Open Google
- Open Facebook
- Open YouTube
- Open Ranchers Cafe

---

##  Music Player

Play songs directly from a predefined music library using voice commands.

Example:

Play Believer

---

##  Exit Command

Safely closes the assistant using voice.

Example:

Exit

---

# Technologies Used

| Category | Technology |
|-----------|------------|
| Language | Python 3 |
| Speech Recognition | SpeechRecognition |
| Text-to-Speech | pyttsx3 |
| Local LLM | Ollama |
| AI Model | Llama 3 |
| Browser Automation | webbrowser |
| Voice Input | Microphone |
| Music Handling | Custom Python Dictionary |
| Conversation Memory | Python List (Chat History) |

---

#  Project Structure

```
Jarvis/
│
├── main.py
├── musicLibrary.py
├── README.md
└── requirements.txt
```

---

#  How It Works

1. Starts microphone listening
2. Waits for wake word "Jarvis"
3. Records user command
4. Detects command type

If it is:

- Browser command → Opens website
- Music command → Plays music
- Exit command → Stops assistant
- Otherwise → Sends prompt to Llama 3

The AI response is converted into speech and spoken back to the user.

---

# AI Workflow

Voice Input

↓

Speech Recognition

↓

Command Processing

↓

If Automation Command

↓

Execute Action

OR

↓

Send Prompt to Llama 3 (Ollama)

↓

Receive AI Response

↓

Text-to-Speech

↓

Voice Output

---

# Example Commands

Open Google

Open YouTube

Open Facebook

Play Believer

What is Artificial Intelligence?

Explain Python Functions

Exit

---

# Future Improvements

- Custom Wake Word Detection
- Offline Speech-to-Text Model
- Better Memory Management
- AI Tool Calling
- File Search
- Desktop Automation
- Smart Home Integration
- RAG Integration
- Vision Capabilities

---

# Installation

Clone the repository

```bash
git clone https://github.com/yourusername/Jarvis.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

Install Ollama

Download Ollama from:

https://ollama.com

Pull Llama 3

```bash
ollama pull llama3
```

Run

```bash
python main.py
```

---

# Requirements

- Python 3.11+
- Ollama
- Llama 3
- Microphone
- Internet (only for Google Speech Recognition)

---

# Learning Outcomes

This project helped me understand:

- Voice AI Applications
- Speech Recognition
- Text-to-Speech
- Local LLM Integration
- Prompt Engineering
- Conversation Memory
- Python Automation
- AI Assistant Architecture

---

# Author

**Madiha Asghar**

BS Computer Science (Gold Medalist)

Management Trainee Officer – Digital Transformation

Passionate about AI, Machine Learning, and Enterprise Systems.

---

 If you like this project, consider giving it a star!
