# 🕵️‍♂️ Criminal Face Recognition System – AI-Powered Surveillance

A real-time AI-powered **Criminal Face Recognition System** designed for smart surveillance and public safety. It uses face detection and face recognition algorithms to identify criminals from a local database using a webcam or phone camera and sends alerts when a match is found.

---

## 🚀 Key Features

- 🎥 **Live Face Detection** via webcam (PC or mobile)
- 🧠 **Local Face Recognition System** – No internet/API required
- ⚠️ **Criminal Alert System** – Visual + audible + SMS notification
- 📲 **Mobile Camera Compatibility** – Supports front and rear
- 📁 **Local Criminal Face Database**
- 🔊 **Alarm Sound** on criminal detection
- 📝 **Add Notes** in database for each entry
- 🔐 **Optimized for Real-World Use**

---

## 📸 How It Works

1. The system opens your camera stream.
2. It scans for faces in real time using **OpenCV + deep learning**.
3. Matches faces with local database using **face encodings**.
4. If a match is found and labeled as “criminal”:
   - An alert message is shown
   - Alarm sound is triggered
   - SMS or notification can be triggered to the authority
5. If the match is labeled as "safe", no alarm is triggered.

---

## 🧪 Technologies Used

- **Frontend:** HTML, CSS, JavaScript (for UI if any)
- **Backend:** Python
- **Libraries:** OpenCV, face_recognition, NumPy, playsound
- **Storage:** Local Face Images (JPG/PNG in folders), optional JSON/CSV
- **Notification:** SMS trigger (optional Twilio/SMTP setup)

---

## 🛠️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Lokesh-kukudala/criminal-face-recognition.git
cd criminal-face-recognition
````

### 2. Create and Activate Virtual Environment

```bash
python -m venv venv
source venv/bin/activate           # Windows: venv\Scripts\activate
```

### 3. Install Required Libraries

```bash
pip install -r requirements.txt
```

If `requirements.txt` is missing, install manually:

```bash
pip install opencv-python face_recognition numpy playsound
```

### 4. Run the Application

```bash
python main.py
```

---

## 📁 Project Structure

```
criminal-face-recognition/
├── known_faces/
│   ├── person1_safe.jpg
│   ├── person2_criminal.jpg
│   └── ...
├── images/
├── static/
├── templates/
├── main.py
├── camera.py
├── database.py
├── utils.py
├── requirements.txt
└── README.md
```

---

## 📂 Face Database Format

Place images of known individuals in `known_faces/`.
Filename convention:

* `name_safe.jpg` → marked as **Safe**
* `name_criminal.jpg` → marked as **Criminal**

System uses filenames to determine alert conditions.

---

## 🔔 Alert System

* ✅ **Safe Person**: Detection with no alert
* ❌ **Criminal**:

  * System shows red alert on screen
  * Alarm sound is triggered
  * Can be extended to send SMS/email alerts to police or family

---

## 📱 Mobile & Real-World Ready

* 📷 Supports rear camera if accessed via mobile browser or connected via IP camera
* ⚡ Lightweight & optimized for minimal lag
* ✅ Cross-platform compatible

---

## 🔐 Privacy & Ethics

* All data is stored and processed **locally**.
* No cloud uploading or third-party services unless configured (e.g., SMS).
* This tool is intended for **educational and surveillance use** only.

---

## 🧠 Future Enhancements

* 📡 Integration with police or criminal records database
* ☁️ Cloud-based dashboard for remote monitoring
* 🧾 Admin panel for face uploads, edits, and notes
* 📲 Android mobile app version

---

## 📌 Limitations

* Requires proper lighting and front-facing image for best accuracy
* Can falsely identify people if low-resolution or side face
* Meant to **assist**, not replace, human verification


## 🤝 Contributing

Pull requests are welcome!

### To Contribute:

```bash
1. Fork the repo
2. Create a new branch: git checkout -b feature-name
3. Make your changes and commit: git commit -m "Description"
4. Push to the branch: git push origin feature-name
5. Open a pull request
```

---

## 📬 Contact

**👤 Lokesh Kukudala**
📧 [kukudalalokesh09@gmail.com](mailto:kukudalalokesh09@gmail.com)
🔗 [GitHub Profile](https://github.com/Nadeem-mohammad0021)

---

> 🔍 Built for smarter surveillance and public safety using AI.
>
> ⚠️ Use responsibly with full compliance to local laws and privacy policies.

```
