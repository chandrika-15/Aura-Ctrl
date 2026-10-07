# Aura-Ctrl

**Aura-Ctrl** is a comprehensive computer control system that allows you to interact with your **Windows PC using hand gestures and voice commands**. Control your mouse, keyboard, applications, and system settings hands-free!

##  Features

- **Gesture Control:** Control mouse cursor, clicks, scrolling, volume, brightness, and launch applications with hand gestures.
- **Voice Control:** Execute commands through speech recognition for app management, window control, and system operations.
- **PowerPoint Integration:** Create and control PowerPoint presentations with voice commands.
- **Cross-Platform UI:** Modern web-based interface for easy access.

##  Prerequisites

Before installing Aura-Ctrl, make sure you have:

- **Operating System:** Windows 10/11
- **Python:** Version 3.8 or higher
- **Camera:** Webcam for gesture control
- **Microphone:** Required for voice control
- **PowerPoint:** Microsoft PowerPoint *(optional, for presentation features)*


##  Installation

### Step 1: Download and Extract

1. Download the Aura-Ctrl project files.
2. Extract the ZIP file to a folder on your computer.

Example:

```text
C:\Aura-Ctrl
```

or

```text
Desktop\Aura-Ctrl
```

### Step 2: Install Python Dependencies

1. Open **Command Prompt** or **PowerShell**.
2. Navigate to the Aura-Ctrl folder:

```bash
cd C:\Path\To\Aura-Ctrl
```

> Replace `C:\Path\To\Aura-Ctrl` with your actual project folder path.

3. Install all required Python packages:

```bash
pip install -r requirements.txt
```

###  Required Python Packages

The project uses the following packages:

| Package | Purpose |
|---|---|
| `opencv-python` | Computer vision and camera processing |
| `mediapipe` | Hand tracking and gesture recognition |
| `numpy` | Numerical computing |
| `pyautogui` | Mouse and keyboard automation |
| `pywin32` | Windows API access |
| `pycaw` | System audio control |
| `comtypes` | COM interface support |
| `screen-brightness-control` | Screen brightness control |
| `PyQt6` | GUI framework |
| `SpeechRecognition` | Speech-to-text |
| `pyttsx3` | Text-to-speech |
| `pywebview` | Web-based interface |
| `google-generativeai` | AI-powered features |
| `pygetwindow` | Window management |

##  Gesture Control

Aura-Ctrl uses **MediaPipe hand tracking** and computer vision to recognize hand gestures and perform computer actions.

### Supported Controls

- ☝️ **Index Finger Up** → Move mouse cursor
- 🤏 **Thumb + Index Pinch** → Mouse click
- ✊ **Fist** → Volume / brightness control
- ✌️ **Index + Middle Fingers** → Scrolling
- 🖐️ **Hand Gestures** → Execute mapped system actions

## 🎙️ Voice Control

Aura-Ctrl allows users to control their computer using voice commands.

### Example Commands

```text
"Open Chrome"
"Close the window"
"Open PowerPoint"
"Start presentation"
"Next slide"
"Previous slide"
"Increase volume"
"Decrease brightness"
```

The available commands depend on the implemented voice-command modules.

## 📊 PowerPoint Integration

Aura-Ctrl provides voice-based PowerPoint control for hands-free presentations.

Features include:

- Create presentations
- Start presentations
- Navigate between slides
- Move to the next slide
- Move to the previous slide
- Control presentations using voice commands

## System Architecture

```text
                    ┌─────────────────────┐
                    │      User Input     │
                    └──────────┬──────────┘
                               │
                 ┌─────────────┴─────────────┐
                 │                           │
                 ▼                           ▼
          ┌─────────────┐             ┌─────────────┐
          │   Webcam    │             │ Microphone  │
          └──────┬──────┘             └──────┬──────┘
                 │                           │
                 ▼                           ▼
          ┌─────────────┐             ┌─────────────┐
          │  MediaPipe  │             │   Speech    │
          │ Hand Tracking│            │ Recognition │
          └──────┬──────┘             └──────┬──────┘
                 │                           │
                 └─────────────┬─────────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Command / Gesture   │
                    │     Processing      │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    System Actions   │
                    └──────────┬──────────┘
                               │
             ┌─────────────────┼─────────────────┐
             ▼                 ▼                 ▼
        Mouse / Keyboard   Applications    System Controls
```

##  Project Structure

```text
Aura-Ctrl/
│
├── README.md
├── requirements.txt
│
├── main.py
├── gesture/
├── voice/
├── powerpoint/
├── ui/
│
├── assets/
└── .gitignore
```

> **Note:** The exact project structure may vary depending on your implementation.

##  Privacy & Security

Aura-Ctrl uses webcam and microphone input for computer interaction.

-  Webcam input is used for hand tracking.
-  Microphone input is used for voice recognition.
-  Do not upload API keys or passwords.
-  Do not commit `.env` files.
-  Use `.gitignore` to protect sensitive files.


##  Use Cases

Aura-Ctrl can be useful for:

-  Accessibility and assistive technology
-  Hands-free computer interaction
-  Smart desktop environments
-  Educational demonstrations
-  Human-Computer Interaction research

