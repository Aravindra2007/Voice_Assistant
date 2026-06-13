# 🤖 JARVIS — Voice Assistant

> **Just a Rather Very Intelligent System**  
> A Python-powered voice assistant inspired by JARVIS from Iron Man, built to automate everyday tasks on your PC/laptop.

---

## 📖 About

JARVIS is a desktop voice assistant that listens to your voice commands and performs a wide range of tasks — from opening applications and playing music, to answering general knowledge questions and checking the weather. It features a clean graphical user interface built with PyQt5.

---

## ✨ Features

- 🗣️ **Greet user** on startup
- 🕐 **Tell current time and date**
- 🚀 **Launch applications/software** on your PC
- 🌐 **Open any website** in your browser
- 🌤️ **Weather updates** for any city (via OpenWeatherMap)
- 📍 **Location & distance finder** — opens maps and tells distance from your location
- 💻 **System status** — RAM usage, battery health, CPU usage
- 📅 **Upcoming events** from Google Calendar
- 📚 **Wikipedia search** — brief info about any person or topic
- 🔍 **Google search** anything
- 🎵 **Play songs on YouTube** by voice
- 📰 **Top headlines** (via Times of India)
- 🎧 **Play local music**
- 📧 **Send emails** with subject and content
- ➗ **Math expression calculator** (e.g., *"Jarvis, calculate x + 135 - 234 = 345"*)
- 🧠 **Answer generic questions** via Wolfram Alpha
- 📝 **Take notes** in Notepad
- 😂 **Tell random jokes**
- 🌐 **Find your IP address**
- 🪟 **Switch windows**
- 📸 **Take screenshots** and save with a custom filename
- 📁 **Hide/unhide files** in a folder
- 🖥️ **Graphical User Interface** built with PyQt5

---

## 🎬 Demo

Watch the project in action: [YouTube Demo](https://www.youtube.com/watch?v=oKtrHy0ERNA)

---

## 🛠️ Built With

- **Python 3.8.5**
- [PyQt5](https://pypi.org/project/PyQt5/) — GUI framework
- [SpeechRecognition](https://pypi.org/project/SpeechRecognition/) — Voice input
- [pyttsx3](https://pypi.org/project/pyttsx3/) — Text-to-speech
- [pywhatkit](https://pypi.org/project/pywhatkit/) — YouTube & WhatsApp automation
- [wikipedia](https://pypi.org/project/wikipedia/) — Wikipedia queries
- [wolframalpha](https://pypi.org/project/wolframalpha/) — Answering general questions
- [psutil](https://pypi.org/project/psutil/) — System resource monitoring
- [geopy](https://pypi.org/project/geopy/) — Location services
- [google-api-python-client](https://pypi.org/project/google-api-python-client/) — Google Calendar integration
- [selenium](https://pypi.org/project/selenium/) — Browser automation

---

## 🔑 API Keys Required

Register and obtain the following API keys before running the project:

| Service | Link |
|---|---|
| OpenWeatherMap | [openweathermap.org/api](https://openweathermap.org/api) |
| Wolfram Alpha | [wolframalpha.com](https://www.wolframalpha.com/) |
| Google Calendar | [developers.google.com/calendar/auth](https://developers.google.com/calendar/auth) |

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Aravindra2007/Voice_Assistant.git
cd Voice_Assistant
```

### 2. Create the Config File

Create a file named `config.py` in the `Jarvis/config/` directory with the following content:

```python
email = "<your_email>"
email_password = "<your_email_password>"
wolframalpha_id = "<your_wolframalpha_id>"
```

### 3. Set Up a Python Virtual Environment

**Using Conda (recommended):**

```bash
conda create -n jarvis python==3.8.5
conda activate jarvis
```

**Or using venv:**

```bash
python -m venv myenv
myenv\Scripts\activate   # Windows
source myenv/bin/activate  # Linux/macOS
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Install PyAudio

PyAudio requires a special installation step. Follow the instructions [here](https://stackoverflow.com/a/55630212) to install it from a wheel file.

### 6. Run the Application

```bash
python main.py
```

---

## 📁 Project Structure

```
Voice_Assistant/
├── Jarvis/
│   ├── config/         # API keys and secret config files
│   ├── features/       # Individual feature modules
│   └── utils/          # GUI assets and images
├── driver/             # Web driver (for Selenium)
├── myenv/              # Python virtual environment
├── gui.ui              # PyQt5 GUI layout file
├── main.py             # Main entry point
├── requirements.txt    # All Python dependencies
├── .gitignore
├── CONTRIBUTING.md
└── LICENSE
```

### Adding a New Feature

1. Create a new `.py` file inside the `Jarvis/features/` folder and write your function.
2. Register the function's definition in `__init__.py`.
3. Add the voice command(s) that should trigger the feature in `main.py`.

---

## 🚀 Future Improvements

- Add NLP-based generalized conversation support
- Improve and modernize the GUI
- Add more smart home / IoT integrations
- Cross-platform support (Linux & macOS)

---

## 🤝 Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on the code of conduct and the process for submitting pull requests.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 👤 Author

**Aravindra2007**  
GitHub: [@Aravindra2007](https://github.com/Aravindra2007)
