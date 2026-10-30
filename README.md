# InterviewHelp 🎯

An intelligent, real-time AI assistant for interviews, technical evaluations, presentations, and meetings. Built with Electron and powered by Google Gemini Live API and Gemini Flash models.

InterviewHelp runs as an unobtrusive, transparent, always-on-top heads-up display (HUD) that listens to interviewer questions directly through your speakers/microphone and provides contextual answers, key bullet points, and code solutions in real time.

---

## 📥 Direct Download (Windows)

No Node.js or development environment required! Download the pre-built Windows installer:

👉 **[Download InterviewHelp-Setup-0.8.0.exe](https://github.com/Akash05-kr/InterviewHelp/releases/download/v0.8.0/InterviewHelp-Setup-0.8.0.exe)** *(~103 MB)*

1. Download and run **`InterviewHelp-Setup-0.8.0.exe`**.
2. Open **Settings** inside the app.
3. Paste your free Gemini API key from [Google AI Studio](https://aistudio.google.com/apikey).
4. Click **Start Session** and you're ready!

---

## ✨ Features

- **🎙️ Real-Time Listening & Transcription**: Listens to the speaker/interviewer in real time using Google Gemini Multimodal Live API over WebSockets.
- **🔊 Speaker Audio Loopback (Windows)**: Directly captures the interviewer's voice from meeting platforms (Zoom, Google Meet, Teams, Discord, etc.) via system loopback.
- **🖼️ Screen & Code Context Analysis**: Instantly captures and analyzes your screen/IDE to help solve algorithmic problems, debug code, or answer questions with full visual context.
- **👻 Stealth / Invisible Overlay**:
  - Always-on-top floating teleprompter.
  - Transparent background with adjustable opacity.
  - Click-through mode (`Ctrl + M`) to click through the overlay without disturbing your active windows.
  - Hidden from taskbar and screen-sharing recordings.
- **⚡ Dual AI Engine Support**:
  - **Google Gemini**: Gemini Multimodal Live API (`gemini-3.1-flash-live-preview` / `gemini-2.5-flash-native-audio-latest`) for real-time conversation + `gemini-3.5-flash` for high-speed screen vision analysis.
  - **Groq (Optional)**: Ultra-fast low-latency responses powered by Llama 3 / Qwen models.
- **🎯 Interview Profiles**: Tailored system instructions for Technical Interviews, System Design, Coding Challenges, Sales Calls, and Exams.

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher)
- A **Gemini API Key** from [Google AI Studio](https://aistudio.google.com/apikey) (Free)
- *(Optional)* A **Groq API Key** from [Groq Console](https://console.groq.com/keys)

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Akash05-kr/InterviewHelp.git
   cd InterviewHelp
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Start the application**:
   ```bash
   npm start
   ```
   *(On Windows PowerShell, you can also run `npm.cmd start`)*

4. **Build Windows Installer (`.exe`)**:
   ```bash
   npm run make
   ```
   The installer package will be output to the `out/make` directory.

---

## ⚙️ Configuration & Usage

1. **Enter API Keys**:
   - On first launch, open the settings menu and paste your **Gemini API Key**.
   - *(Optional)* Add a Groq API Key for instant response generation.
   - Keys are securely stored locally on your machine and never tracked in the repository.

2. **Audio Mode**:
   - Select **Speaker Only** to capture the interviewer's voice through your system audio.
   - Select **Both** to capture both your microphone and the interviewer's voice.

3. **Start Session**:
   - Click **Start Session**.
   - Position the teleprompter window near your webcam for natural eye contact.

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| `Ctrl + Arrow Keys` | Move the overlay window |
| `Ctrl + M` | Toggle click-through mode (ignore mouse clicks) |
| `Ctrl + \` | Close window or go back |
| `Ctrl + Enter` | Trigger manual screenshot analysis |
| `Enter` | Send custom text prompt to AI |

---

## 🛡️ Privacy & Security

- **Local Storage**: API credentials and configuration settings are stored locally in your operating system's application data directory (`%APPDATA%/cheating-daddy-config/` on Windows) and are ignored by Git.
- **Protection**: Screen capture content protection is enabled to prevent the overlay itself from appearing in screen shares where supported.

---

## 📄 License

This project is licensed under the [GPL-3.0 License](LICENSE).
