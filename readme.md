# 🤖 MockMate

**MockMate** is an AI-powered mock interview platform that bridges the gap between preparation and performance. By combining Large Language Models, real-time emotion recognition, and digital human avatars, MockMate provides an immersive environment to sharpen your interview skills.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![Flask](https://img.shields.io/badge/framework-Flask-lightgrey.svg)](https://flask.palletsprojects.com/)

---

## 🚀 Overview

Preparing for interviews is often a lonely and static process. **MockMate** changes that by offering:
* **Resume & JD Intelligence**: Upload your resume and the job description to find exactly where you stand.
* **Realistic Simulations**: Choose between a text-based AI chat or a high-fidelity video interview with an AI avatar.
* **Emotional Intelligence**: Get feedback not just on *what* you said, but *how* you looked while saying it.

---

## 🛠️ Tech Stack

| Category | Tools & Technologies |
| :--- | :--- |
| **Backend** | Python (Flask), SQLite, SQLAlchemy |
| **AI / LLM** | LangChain, Google Gemini API, Ollama (Local LLM) |
| **Computer Vision** | FER (Facial Emotion Recognition), OpenCV |
| **Document Processing** | EasyOCR, PyMuPDF (Fitz) |
| **Avatar Synthesis** | HeyGen Streaming API |
| **Frontend** | Jinja2, Tailwind CSS, JavaScript |

---

## 🖼️ Feature Gallery

### 1. Analysis & Preparation
MockMate extracts text from your documents (using **OCR** for scanned images and **PyMuPDF** for text layers) to identify "Skill Gaps."

| JD & Resume Analysis | Skill Gap & Study Plan |
| :---: | :---: |
| ![JD Analysis](screenshots/6.analyze1.png) | ![Skill Gap](screenshots/7.skillgapanalysis.png) |

### 2. The Interview Experience
Toggle between a standard technical interface and a lifelike avatar interaction powered by the HeyGen API.

| Avatar-Driven Interview | Technical Coding Interview |
| :---: | :---: |
| ![Avatar Interview](screenshots/9.avatar.png) | ![Coding Interview](screenshots/10.coding.png) |

### 3. Tracking Progress
The dashboard saves every session, allowing you to track your improvement over time with detailed emotional and logic scores.

| Main Dashboard | Performance Analytics |
| :---: | :---: |
| ![Dashboard 1](screenshots/3.dashboard1.png) | ![Dashboard 2](screenshots/5.dashboard3.png) |

---

## ⚙️ Installation & Setup

### Prerequisites
* Python 3.9 or higher
* A webcam (for Emotion Recognition)
* An active internet connection (for Gemini/HeyGen APIs)

### Step-by-Step Setup

1.  **Clone the Repository**
    ```bash
    git clone [https://github.com/KB1118/MockMate_Smart_Avatar_Mock_Interview.git](https://github.com/KB1118/MockMate_Smart_Avatar_Mock_Interview.git)
    cd MockMate_Smart_Avatar_Mock_Interview
    ```

2.  **Create a Virtual Environment** (Recommended)
    ```bash
    python -m venv venv
    # Windows:
    venv\Scripts\activate
    # Mac/Linux:
    source venv/bin/activate
    ```

3.  **Install Dependencies**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Configure Environment Variables**
    Create a `.env` file in the root directory:
    ```env
    SECRET_KEY=your_flask_secret_key
    GOOGLE_API_KEY=your_gemini_api_key
    HEYGEN_API_KEY=your_heygen_api_key
    ```

5.  **Initialize & Run**
    ```bash
    python run.py
    ```
    Visit `http://localhost:5000` in your browser.

---

## 💡 Troubleshooting

* **Webcam Not Found**: Ensure no other application (like Zoom or Teams) is using your camera. Browser permissions must be set to "Allow."
* **Ollama Issues**: If using local models, ensure the Ollama service is running in the background before launching the app.
* **Database Reset**: If you encounter schema errors, you can safely delete `instance/chat.db` to let the app regenerate a fresh database.

---

## 🤝 Contributing

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.

---
_Last updated: December 2025_
