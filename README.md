# Safe-Guard-Helmet
Your companion for ultimate protection.


## Overview
**NIRBHAYA: The Securix** is a **basic prototype** of a women safety desktop application built entirely in **Python** — without any login or cloud integration.  
It is designed to **assist in emergency or unsafe situations** by integrating simple real-time features like **face detection**, **emotion analysis**, **audio recording**, and **location tracking**, all wrapped in a clean **PyQt6-based GUI**.

This project is a foundation version of the *NIRBHAYA* system and can be further expanded into a full-fledged smart safety assistant with cloud storage, authentication, alert systems, and AI integration.

---

##  Features
### Core Functionalities
1. **Face Detection (OpenCV)**  
   - Real-time face detection using the webcam.  
   - Draws green rectangles around detected faces.  
   - Press `Q` to quit the camera window.  

2. **Emotion Detection (MediaPipe)**  
   - Uses **MediaPipe FaceMesh** to analyze facial landmarks.  
   - Detects basic emotions: `Happy`, `Neutral`, `Sad`, `Nervous`.  
   - Displays emotion text overlay on the live camera feed.  

3. **Audio Recording & Playback (sounddevice)**  
   - Record voice/audio for a fixed duration (default 5 seconds).  
   - Saves the recording as `voice_recording.wav`.  
   - Playback feature available (currently Windows supported).  

4. **GPS Location Detection (geocoder)**  
   - Fetches the approximate **latitude** and **longitude** using the user’s IP.  
   - Displays coordinates via popup dialog in the GUI.  

---

##  Tech Stack
| Category | Tools / Libraries Used |
|-----------|------------------------|
| **GUI Framework** | PyQt6 |
| **Computer Vision** | OpenCV |
| **Facial Landmark Detection** | MediaPipe |
| **Audio Handling** | sounddevice, scipy.io.wavfile |
| **Location Tracking** | geocoder |
| **Core Language** | Python 3.8+ |

---

##  How It Works
1. Launch the app using the Python script.  
2. The GUI window provides buttons for each feature.  
3. Click on any feature to activate it:  
   - `Start Face Detection`: Opens camera feed with face detection.  
   - `Detect Emotion`: Analyzes and displays live emotion on the camera feed.  
   - `Record Voice`: Records audio for 5 seconds.  
   - `Play Recording`: Plays the recorded audio file.  
   - `Show Location`: Displays current latitude and longitude in a popup.  

---

##  Installation & Setup

###  Prerequisites
- Python 3.8 or later  
- A webcam and microphone  
- Windows or Linux (Mac may require minor tweaks)

###  Required Libraries
Install all dependencies using pip:

```bash
pip install opencv-python sounddevice scipy geocoder mediapipe PyQt6
