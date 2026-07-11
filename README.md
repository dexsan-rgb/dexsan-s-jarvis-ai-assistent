Markdown
# JARVIS AI Assistant 🚀

An advanced, light-weight, and custom voice assistant with hybrid capabilities. It can run in standard mode or conversational mode using the Hugging Face Inference API, with a local backend search fallback if the API is offline.

---

## 🌟 Key Features
- **Double Clap Wakeup:** Wakes up from deep sleep on detecting a double clap and the correct passphrase.
- **Hybrid AI Core:** Connects to Hugging Face (`zephyr-7b-beta`) for intelligent replies, and falls back seamlessly to offline-style DuckDuckGo API/Wikipedia scraping to summarize answers instantly.
- **Smart Conversations:** Full continuous speech interaction in "Conversational Mode".
- **System Commands:** Open Arduino IDE, VirtualBox, Chrome, play YouTube videos, and control system volume/brightness.
- **Battery Monitoring:** Automatically tracks power status and alerts you when the battery drops below 20%.

---

## 🛠️ Prerequisite Installation 

This project requires **Python 3.x**. Before running `jarvis.py`, you must install the following dependencies using your terminal or Command Prompt / PowerShell:


# 1. Sound & Voice Recognition Libraries
pip install sounddevice scipy SpeechRecognition gTTS playsound==1.2.2

# 2. Mathematical & OS Tracking Utilities
pip install numpy psutil

# 3. System Automation & Screen Controls
pip install screen-brightness-control pyautogui

# 4. Optional: Automation for YouTube
pip install pywhatkit
📌 Note for Linux/Kali Users: If you are running this on Linux, you might need to install portaudio before running the pip commands:
sudo apt update && sudo apt install portaudio19-dev

🚀 How to Run
Follow these exact steps to start JARVIS on your machine:

Step 1: Download or clone this repository to your local machine.
Step 2: Open your Terminal or PowerShell and navigate to the folder where jarvis.py is saved.
Step 3: Run the script using Python:
python jarvis.py

Step 4: Once the terminal says Jarvis Master Core: Monitoring Active... [Clap to Wake Up]:

Give a Double Clap 👏 👏.
Wait for it to print Awaiting reality phrase...
Say "wake up" or "reality" to fully activate JARVIS.

🎙️ Voice Commands Guide:
"Conversational mode" - Switches to a continuous full-AI voice call experience.
"Stop conversation" - Returns to standard command mode.
"Play [Song Name] on YouTube" - Automatically opens and plays the video.
"Go to sleep" - Puts JARVIS back into power-saving deep sleep mode.