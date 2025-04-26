
# 🚨 Scam Detector Web App

A Flask-based web application that uses Google's **Gemini AI model** to detect scam content in text files and classify suspicious URLs. This tool helps identify whether a given **email or text is legitimate or a scam**, and whether a **URL is benign, phishing, malware, or defacement**.

---

## 🌐 Features

- 🔍 **Email/Text Scam Detection**: Upload a `.pdf` or `.txt` file and let the model classify it as **Real** or **Scam**.
- 🌐 **URL Classification**: Input a URL to get its classification — **benign**, **phishing**, **malware**, or **defacement**.
- 🤖 Powered by **Gemini 1.5 Flash** from Google AI.
- 🖥️ Simple and clean user interface with Flask and HTML templates.

---

## 🧠 Tech Stack

- Python
- Flask
- Google Generative AI (Gemini)
- PyPDF2
- HTML (Jinja Templates)

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/scam-detector.git
cd scam-detector
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

<details>
<summary><strong>requirements.txt (example)</strong></summary>

```
Flask
google-generativeai
PyPDF2
```

</details>

### 3. Set Google API Key

Create an `.env` file or export the key directly in your terminal:
```bash
export GOOGLE_API_KEY=your_api_key_here
```

> Replace `your_api_key_here` with your actual API key from Google AI Studio.

### 4. Run the App
```bash
python main.py
```

The app will start at: `http://127.0.0.1:5000`

---

## 🧪 How to Use

### 🔤 Detect Email or Text Scams
- Go to `/scam/`
- Upload a `.pdf` or `.txt` file
- Get instant classification

### 🔗 Predict URL Safety
- Go to `/predict`
- Enter a URL (must start with `http://` or `https://`)
- View the result on the same page

---

## 📂 Project Structure

```
├── main.py               # Main Flask application
├── templates/
│   └── index.html        # Web interface
├── static/               # Optional static assets
└── requirements.txt      # Python dependencies
```

---

## ⚠️ Disclaimer

This project uses an AI model for text classification, which **may not always be 100% accurate**. Always double-check critical decisions with professional tools.

---

## 🛠 Future Improvements

- Add user authentication
- Save scan history
- Support for other file types (e.g., DOCX)
- Enhanced UI/UX with Bootstrap or Tailwind
