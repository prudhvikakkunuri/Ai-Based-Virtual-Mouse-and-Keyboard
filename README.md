# 🖐️🖥️ Virtual Mouse & Keyboard using Hand Gesture Recognition

A real-time Computer Vision project that enables touchless human–computer interaction using hand gestures.  
This system replaces traditional input devices such as a mouse and keyboard with a gesture-based virtual interface powered by MediaPipe and OpenCV.

---

# 📌 Table of Contents

- Project Overview
- Business Problem
- Solution Approach
- Features
- Technology Stack
- System Architecture
- Installation Guide
- Usage Instructions
- Gesture Controls
- Working Methodology
- Challenges Faced
- Limitations
- Future Enhancements
- Resume Description

---

# 🚀 Project Overview

Human–Computer Interaction (HCI) traditionally depends on physical devices such as a mouse and keyboard.  
While effective, these devices:

- Require physical contact
- Are not accessible to individuals with mobility limitations
- Pose hygiene risks in sterile environments
- Limit mobility during presentations or public interaction systems

This project introduces a gesture-based virtual mouse and keyboard system that enables users to control a computer using only hand movements captured through a webcam.

The system uses real-time hand landmark detection to interpret gestures and convert them into system-level input actions.

---

# 🏢 Business Problem

Organizations and individuals require safer, more accessible, and hardware-independent interaction systems.

Current challenges include:

- Dependency on physical input devices
- Hygiene concerns in hospitals and laboratories
- Limited accessibility for differently-abled users
- Hardware failure disrupting productivity
- Lack of intuitive natural interaction systems

There is a need for a touchless, intelligent interface that enables natural interaction without physical hardware.

---

# 💡 Solution Approach

This project leverages Computer Vision and AI-based hand tracking to:

- Detect hand landmarks in real-time
- Track index finger movement for cursor control
- Detect pinch gestures for mouse clicks
- Implement a virtual on-screen keyboard
- Detect tapping gestures to trigger key presses
- Map camera coordinates to screen resolution dynamically

The system processes live video frames, extracts hand coordinates, and translates them into operating system input commands using PyAutoGUI.

---

# ✨ Key Features

- 🖱️ Real-time gesture-based mouse control
- 👆 Pinch gesture for left click
- ⌨️ On-screen virtual keyboard
- 📝 Live input text box display
- 🎯 Tap detection for typing
- ⚡ Smooth cursor movement
- 🔁 Cooldown logic to prevent accidental multiple clicks
- 🖥️ Windowed interface with full controls
- 🧠 Real-time hand landmark tracking (21 points)

---

# 🛠️ Technology Stack

- **Python** – Core programming language
- **OpenCV** – Video capture & UI rendering
- **MediaPipe** – Hand landmark detection framework
- **PyAutoGUI** – OS-level mouse and keyboard control
- **NumPy** – Mathematical operations

---

# 🏗️ System Architecture

1. Webcam captures live video feed
2. OpenCV processes each frame
3. MediaPipe detects 21 hand landmarks
4. Index finger coordinates are extracted
5. Coordinate mapping converts camera space to screen space
6. Gesture detection logic identifies:
   - Pinch gesture → Mouse click
   - Tap gesture → Keyboard input
7. PyAutoGUI sends system-level commands

---

# 📦 Installation Guide

## Step 1: Create Virtual Environment

```bash
python -m venv venv
venv\Scripts\activate
```

## Step 2: Install Required Dependencies

```bash
python vmouse.py
```
