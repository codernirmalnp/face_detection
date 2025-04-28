# Face Detection and Alert System

This project is a **Flask-based** real-time **face detection and recognition** system from an **RTSP camera feed**, using **OpenCV**, **face_recognition**, and **Flask-SocketIO**. It manages users, faces, and alerts through a simple web dashboard.

---

## Features
- 📸 Real-time RTSP video streaming using FFmpeg
- 🧠 Detect and recognize familiar faces
- 🔔 Send real-time alerts for familiar/unfamiliar faces
- 🧩 Web admin panel to add known faces
- 📚 User authentication (login/logout)
- 🗂️ View and filter face alerts by type and date
- 🧵 Background alert processing for better performance

---

## Technologies Used
- Python 3.8+
- Flask
- Flask-SocketIO
- OpenCV
- face_recognition
- SQLAlchemy (ORM)
- SQLite
- FFmpeg

---

## Installation Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/codernirmalnp/face_detection.git
cd face_detection
