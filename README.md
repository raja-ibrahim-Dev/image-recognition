# 📸 AI-Powered Attendance System using Face Recognition

A mobile-based attendance solution that uses computer vision to automate student identification and record attendance. Built with a fine-tuned ResNet-50 model, served via FastAPI, and integrated into a Flutter mobile app with Firebase backend.

---

## 🚀 Features

- 🎓 Teachers can create and manage lectures via mobile
- 🤳 Students capture a selfie to mark attendance
- 🧠 Face recognition using fine-tuned ResNet-50
- ☁️ Model hosted as an API on Hugging Face Spaces
- 🔥 Attendance stored in Firebase Firestore

---

## 🧠 Model

- **Architecture:** ResNet-50 (pre-trained)
- **Fine-tuning:** Custom dataset with 31 classes (one per person)
- **Dataset:** [Face Recognition Dataset – Kaggle](https://www.kaggle.com/datasets/vasukipatel/face-recognition-dataset/data)
- **Framework:** PyTorch
- **Deployment:** FastAPI app hosted on Hugging Face Spaces

---

## 📱 Mobile App

- **Framework:** Flutter
- **Functionality:**
  - Open camera
  - Send image to backend API
  - Display prediction result
  - Record attendance in Firebase
- **Backend Communication:** REST API (image sent via `multipart/form-data`)

---

## 🛠 Tech Stack

| Technology     | Purpose                        |
|----------------|--------------------------------|
| PyTorch        | Model training & fine-tuning   |
| FastAPI        | Model serving via REST API     |
| Hugging Face   | API hosting                    |
| Flutter        | Cross-platform mobile app      |
| Firebase       | Real-time database for logs    |

---

## 📂 Project Structure

```
📁 Backend/
│   ├── app.py              # FastAPI backend
│   ├── model.pth           # Trained model weights
│   ├── classes.txt         # Label names
│   └── requirements.txt    # Dependencies
📁 Recognition/
│   ├── lib/
│   ├── android/
│   └── pubspec.yaml        # Flutter dependencies
```

---

## ✅ How to Run

### 🔧 Backend

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Run API server:
   ```bash
   uvicorn app:app --reload
   ```

### 📱 Flutter App

1. Install dependencies:
   ```bash
   flutter pub get
   ```
2. Run app:
   ```bash
   flutter run
   ```

---

## 📊 Results

- High accuracy on known faces
- Real-time recognition in mobile app
- Reliable attendance logging

---

## 📚 References

- [Kaggle Dataset](https://www.kaggle.com/datasets/vasukipatel/face-recognition-dataset/data)
- [ResNet Paper](https://arxiv.org/abs/1512.03385)
- [PyTorch Docs](https://pytorch.org)
- [FastAPI Docs](https://fastapi.tiangolo.com)
- [Flutter Docs](https://flutter.dev)
- [Firebase Docs](https://firebase.google.com)

---

## 🙌 Acknowledgments

Built by [Your Name] using cutting-edge open-source tools and frameworks.
