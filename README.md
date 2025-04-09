# Chiron: File Query System

Chiron is a file-based question-answering system that allows users to upload various document types (PDF, DOCX, TXT, XLSX, JSON) and ask questions based on the content of those files.

---

## 🧠 Features

- Upload and parse documents on the backend
- Ask natural language questions related to uploaded content
- Instant responses in a ChatGPT-style UI
- Responsive and modern interface

---

## 🛠️ Local Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/chiron.git
cd chiron
```

---

### 2. Setup Python Environment

```bash
cd backend
python -m venv venv
venv\Scripts\activate   # On Windows
# OR
source venv/bin/activate  # On macOS/Linux

pip install -r requirements.txt
```

---

### 3. Install Required Packages

Make sure your `requirements.txt` contains:

```
flask
flask-cors
python-docx
openpyxl
PyPDF2
```

---

### 4. Run Flask Server

```bash
python app.py
```

The backend will start on `http://127.0.0.1:5000`

---

### 5. Open the Frontend

Open `frontend/index.html` directly in your browser or use a local server like:

```bash
cd frontend
python -m http.server
```

Then visit `http://localhost:8000`

> Make sure your `script.js` file uses the correct local endpoint:
```js
fetch('http://127.0.0.1:5000/upload')
```

---

## 📸 Screenshots

> (Insert screenshots or gifs showing UI, file upload, and querying in action)

---

## 📌 Notes

- Max file size: 50 MB
- Supported formats: `.pdf`, `.docx`, `.xlsx`, `.txt`, `.json`
- Cross-origin support enabled using Flask-CORS

---

## 📄 License

MIT License – free to use with attribution.
