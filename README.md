# 🧠 Steel Surface Defect Detection App

A complete end-to-end mobile application for detecting steel surface defects using deep learning. Built with **Flutter** for the frontend and **PyTorch** for backend inference, this project enables users to capture or upload images of steel and receive real-time predictions of surface defects.

---

## 📱 Features

- 📷 Capture or upload steel surface images via camera.
- 🤖 Deep learning model (Faster R-CNN) for defect detection.
- 📊 Bounding box visualization for predicted defects.
- 💾 History of previous scans stored locally.
- ✉️ Email verification and authentication (optional).
- 🌐 Backend powered by Python & Node.js.
- 🔍 Differentiates between steel and non-steel objects.

---

## 🧠 Defect Classes

The model can detect the following surface defects:

- Crazing
- Inclusion
- Pitted Surface
- Scratches
- Rolled-in Scale
- Patches

---

## 🛠️ Tech Stack

| Layer          | Technology                         |
|---------------|-------------------------------------|
| Frontend      | Flutter                             |
| Backend API   | Node.js (Express)                   |
| ML Model      | PyTorch (Faster R-CNN)              |
| Image Upload  | Multer (Node.js)                    |
| Model Serving | Python script via subprocess        |
| Auth          | Firebase or Clerk (configurable)    |

---

## 🚀 How It Works

1. 📲 User captures or uploads a steel surface image.
2. 📡 Image is sent to the backend.
3. 🧠 Backend loads the trained PyTorch model and runs inference.
4. 📍 Predictions and bounding boxes are returned to the app.
5. 🖼️ Bounding boxes and defect labels are visualized in-app.

---

## 📦 Folder Structure

steel-defect-detection/
│
├── frontend/ # Flutter app code
├── backend/ # Node.js + Python backend
│ └── predict.py # Python model inference
├── models/ # PyTorch model files
└── assets/ # Logo and UI assets


## 🧪 Model Training

The model was trained on [NEU Surface Defect Database](https://github.com/idealplayer/NEU-CLS) and CIFAR-10 (for steel-vs-non-steel classification), using:

- Epochs: 50+
- Optimizer: SGD / Adam
- Confidence threshold: 0.65
- Backbone: ResNet-50 + FPN

---

## ✨ Screenshots

| Home | Detection | Bounding Boxes |
|------|-----------|----------------|
| ![Home](assets/screens/home.png) | ![Detect](assets/screens/results.png) | ![Boxes](assets/screens/bbox.png) |

---

## 🧰 Requirements

### Frontend
- Flutter SDK
- `image_picker`, `http`, `provider`, etc.

### Backend
- Node.js
- Python 3.x
- PyTorch
- torchvision
- Flask / subprocess module

---

## 🤝 Contributing

Feel free to fork this repo, open issues, and submit PRs.
If you improve the model, UI/UX, or backend efficiency, contributions are welcome!

---

## 📜 License

This project is licensed under the MIT License.

---

## 📬 Contact

Developed by Hammad Khattak
📧 Email: hk1630686@gmail.com  
🏫 COMSATS University, Abbottabad
