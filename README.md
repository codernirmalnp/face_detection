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


2. Create and Activate a Virtual Environment
bash
Copy
Edit
python -m venv venv
# On Linux/macOS:
source venv/bin/activate
# On Windows:
venv\Scripts\activate



. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
Make sure flask, flask-socketio, flask-sqlalchemy, flask-migrate, face-recognition, opencv-python and other packages are installed.

Environment Variables Setup
You must create a .env file in the root directory (NOT committed to GitHub).

Example .env file:

env
Copy
Edit
ADMIN_USERNAME=youradminusername
ADMIN_PASSWORD=youradminpassword
RTSP_URL=your_rtsp_stream_url
⚠️ Never upload .env to your GitHub repository!

FFmpeg Setup
Ensure that the bin/ directory exists and contains the ffmpeg.exe file.
If not, download FFmpeg from ffmpeg.org and place the ffmpeg.exe inside the bin/ folder.

Example folder structure:

cpp
Copy
Edit
face_detection/
├── app.py
├── bin/
│   └── ffmpeg.exe
├── models.py
├── extensions.py
├── templates/
├── static/
├── app.db
└── requirements.txt
Running the Application
Start the Flask server locally:

bash
Copy
Edit
python app.py
Then open your browser and go to:

cpp
Copy
Edit
http://127.0.0.1:5000
✅ Login with the credentials you set in your .env file.

Usage Guide
📷 Live Video Feed: View real-time face recognition from your camera.

➕ Add Known Faces: Upload face images from the admin panel (/add_known_face).

🔔 View Alerts: See the list of alerts, filtered by familiar or unfamiliar detections (/alerts).

🔒 Authentication: Protects admin features (login/logout).

Project Structure
plaintext
Copy
Edit
face_detection/
│
├── app.py              # Main Flask application
├── models.py           # SQLAlchemy models (User, Face, Alert)
├── extensions.py       # Database connection
├── templates/          # HTML templates (Jinja2)
├── static/             # Static files (CSS, JS, images)
├── bin/
│   └── ffmpeg.exe      # FFmpeg for RTSP streaming
├── app.db              # SQLite database
├── requirements.txt    # Python dependencies
├── README.md           # Project documentation
└── .env                # (You create this manually, not uploaded)
GitHub Instructions
When you make any changes:

bash
Copy
Edit
git add .
git commit -m "Your commit message"
git push origin main
Replace main with your branch name if it's different.

Database Migration Commands
If you change the database models (models.py), follow these steps:

1. Initialize Migrations (only first time)
bash
Copy
Edit
flask db init
2. Generate Migration Scripts
bash
Copy
Edit
flask db migrate -m "Describe the change"
3. Apply Changes to Database
bash
Copy
Edit
flask db upgrade
✅ Flask-Migrate must be installed:

bash
Copy
Edit
pip install Flask-Migrate
This keeps your database schema updated without deleting existing data.

License
This project is licensed under the MIT License.

🚀 Happy Coding!
yaml
Copy
Edit

---

✅ This version includes **everything** you asked for.  
✅ It looks clean, complete, and ready for **real open-source/public** or **private** use.

---

Would you also like me to generate a **real ready `requirements.txt` file** based on your imports too?  
I can give you that in 5 seconds if you want 📦✅.  
Would you like me to send it? 🚀








