# 🤖 JARVIS Voice Assistant

**Just A Rather Very Intelligent System** — a Python-based desktop voice assistant inspired by Iron Man's JARVIS. Built to automate everyday tasks on your PC using voice commands, featuring a sleek PyQt5 GUI.

---

## ✨ Features

- 🕐 **Date & Time** — Ask for the current time or date at any moment
- 🌦️ **Weather** — Get live weather updates for any city
- 🚀 **App Launcher** — Launch applications on your PC by voice
- 🌐 **Website Opener** — Open any website instantly
- 📍 **Location & Distance** — Find any place and get the distance from your current location
- 📰 **Top Headlines** — Fetches the latest news from Times of India
- 🎵 **Music & YouTube** — Play local music or any video on YouTube
- 📧 **Send Emails** — Compose and send emails hands-free
- 🧮 **Math & General Q&A** — Powered by WolframAlpha for calculations and general queries
- 📖 **Wikipedia Lookup** — Get summaries about any person or topic
- 📅 **Google Calendar** — Check upcoming events and plans
- 📝 **Notes** — Take and save voice notes in Notepad
- 😂 **Jokes** — Ask for a random joke
- 🖥️ **System Info** — Check RAM usage, battery health, and CPU usage
- 🌍 **IP Address** — Retrieve your current public IP
- 🖼️ **Screenshots** — Take and save screenshots with a custom filename
- 🗂️ **Hide/Show Files** — Toggle visibility of all files in a folder
- 🔀 **Window Switcher** — Switch between open windows by voice
- 🖼️ **Animated GUI** — A live animated PyQt5 interface with a real-time clock

---

## 🛠️ Built With

- **Python 3.8+**
- **PyQt5** — GUI framework
- **SpeechRecognition / PyAudio** — Voice input
- **pyttsx3 / gTTS** — Text-to-speech
- **WolframAlpha API** — Computational intelligence
- **OpenWeatherMap API** — Weather data
- **Google Calendar API** — Calendar events
- **pywhatkit** — YouTube playback
- **pyjokes** — Joke generation
- **Wikipedia API** — Topic lookups
- **pyautogui** — Screenshot & window switching

---

## 📋 Prerequisites

- Python 3.8 or higher
- A working microphone
- Anaconda (recommended) or a standard Python virtual environment

---

## 🔑 API Keys Required

Register and obtain API keys from the following services before running the project:

| Service | Link |
|---|---|
| OpenWeatherMap | https://openweathermap.org/api |
| WolframAlpha | https://www.wolframalpha.com/ |
| Google Calendar | https://developers.google.com/calendar/auth |

---

## 🚀 Installation

**1. Clone the repository**

```bash
git clone https://github.com/Aravindra2007/Voice_Assistant.git
cd Voice_Assistant
```

**2. Create and activate a virtual environment**

Using Anaconda (recommended):
```bash
conda create -n jarvis python==3.8.5
conda activate jarvis
```

Or using standard venv:
```bash
python -m venv myenv
# Windows
myenv\Scripts\activate
# macOS/Linux
source myenv/bin/activate
```

**3. Install dependencies**

```bash
pip install -r requirements.txt
```

For PyAudio on Windows, install from a wheel file. See [this StackOverflow answer](https://stackoverflow.com/a/55630212) for instructions.

**4. Configure API keys**

Create a file at `Jarvis/config/config.py` with the following content:

```python
email = "<your_email>"
email_password = "<your_email_password>"
wolframalpha_id = "<your_wolframalpha_app_id>"
```

**5. Run the assistant**

```bash
python main.py
```

---

## 🗂️ Project Structure

```
Voice_Assistant/
├── Jarvis/
│   ├── config/         # API keys and configuration
│   ├── features/       # Individual feature modules
│   └── utils/          # GUI assets and images
├── driver/             # Driver utilities
├── myenv/              # Virtual environment (excluded from git)
├── gui.ui              # PyQt5 UI layout file
├── main.py             # Main entry point
├── requirements.txt    # Python dependencies
├── .gitignore
├── LICENSE
├── CONTRIBUTING.md
└── README.md
```

---

## 🎤 Example Voice Commands

| Command | Action |
|---|---|
| `"Hey Jarvis"` / `"Wake up Jarvis"` | Wake / greet the assistant |
| `"What's the time?"` | Tells current time |
| `"What's the date?"` | Tells today's date |
| `"Weather in [city]"` | Fetches weather for a city |
| `"Open [website]"` | Opens a website in the browser |
| `"Launch Chrome"` | Launches an application |
| `"Tell me about [topic]"` | Wikipedia summary |
| `"What is [question]?"` | WolframAlpha answer |
| `"Play [song] on YouTube"` | Plays video on YouTube |
| `"Send email"` | Initiates email composition |
| `"Top headlines"` / `"News"` | Reads today's top news |
| `"Take a screenshot"` | Captures and saves the screen |
| `"Tell me a joke"` | Tells a random joke |
| `"System status"` | Reports CPU, RAM, and battery |
| `"Where is [place]?"` | Location and distance info |
| `"Goodbye"` / `"Bye"` | Shuts down the assistant |

---

## 🔧 Adding New Features

The codebase is modular and easy to extend:

1. Create a new `.py` file inside `Jarvis/features/` with your feature function.
2. Register the function in `Jarvis/__init__.py`.
3. Add the voice command trigger(s) inside the `TaskExecution` loop in `main.py`.

---

## 🤝 Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for the code of conduct and the process for submitting pull requests.

---

## 🔮 Future Improvements

- Natural Language Processing for more fluid, open-ended conversations
- Enhanced and more interactive GUI
- Cross-platform support (Linux & macOS)
- Expanded application launcher with auto-detection
- Smarter context memory across commands

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
