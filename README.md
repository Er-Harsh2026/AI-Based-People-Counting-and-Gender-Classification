# 🚀 AI-Based People Counting and Gender Classification

An AI-powered video analytics system that detects, tracks, and counts people moving from **Left → Right** across a user-defined polygon region. The project also performs **gender classification** using AI whenever a clear face is detected.

---

## 📌 Project Overview

This project was developed as part of the **PROACT AI Assignment**.

The system uses **YOLO11** for person detection, **ByteTrack** for multi-object tracking, and **InsightFace** for gender classification. It counts only unique people crossing a predefined Region of Interest (ROI) from **Left to Right**, while displaying live statistics on the output video.

---

## ✨ Features

- ✅ Person Detection using YOLO11
- ✅ Multi-Object Tracking using ByteTrack
- ✅ Polygon-based ROI Selection
- ✅ Left → Right People Counting
- ✅ Gender Classification (Male/Female)
- ✅ Live Track ID Display
- ✅ Real-time Male, Female & Total Counter
- ✅ CSV Report Generation
- ✅ Annotated Output Video
- ✅ Duplicate Count Prevention

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Python 3.11 | Programming Language |
| YOLO11 | Person Detection |
| ByteTrack | Multi-Object Tracking |
| InsightFace | Gender Classification |
| OpenCV | Video Processing |
| PyTorch | Deep Learning |
| NumPy | Numerical Operations |
| Pandas | CSV Report |
| Shapely | Polygon Operations |
| Matplotlib | Visualization |

---

## 📂 Project Structure

```
PROACT_AI_Assignment/
│
├── Assignment.ipynb
├── TownCentreXVID.mp4
├── yolo11n.pt
├── output.mp4
├── People_Count.csv
├── README.md
└── requirements.txt
```

---

## ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

Move to the project directory

```bash
cd YOUR_REPOSITORY
```

Install all dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ How to Run

1. Open **Assignment.ipynb** in Jupyter Notebook or VS Code.
2. Download the YOLO11 model (`yolo11n.pt`) and place it in the project folder.
3. Keep the input video (`TownCentreXVID.mp4`) in the same directory.
4. Run all notebook cells sequentially.
5. The processed video and CSV report will be generated automatically.

---

## 🔄 Workflow

```
Input Video
      │
      ▼
YOLO11 Person Detection
      │
      ▼
ByteTrack Tracking
      │
      ▼
Polygon Crossing Detection
      │
      ▼
Face Detection
      │
      ▼
Gender Classification
      │
      ▼
Male Count
Female Count
Total Count
      │
      ▼
CSV Report + Output Video
```

---

## 📊 Output

### 🎥 Output Video

The generated video contains:

- Person Bounding Boxes
- Track IDs
- Gender Labels
- Polygon Region
- Live Male Count
- Live Female Count
- Total People Count

---

### 📄 CSV Report

The system generates a CSV report containing:

| Frame | Track ID | Gender | Direction |
|--------|----------|---------|-----------|
| 245 | 8 | Male | Left_to_Right |
| 382 | 15 | Female | Left_to_Right |

---

## ⚠️ Limitations

- Gender classification depends on face visibility.
- Small, blurred, or occluded faces may not be classified correctly.
- The system is optimized for Left → Right movement across the selected polygon.

---

## 🚀 Future Improvements

- Age Prediction
- Face Recognition
- Emotion Detection
- Real-time Webcam Support
- Person Re-Identification
- Dashboard Analytics
- Multi-directional Counting

---

## 👨‍💻 Developed By

**Harsh Mishra**

B.Tech Computer Science & Engineering

MCKV Institute of Engineering

---

## 📜 License

This project was developed for educational and assignment purposes.

---

⭐ If you found this project useful, consider giving it a **Star** on GitHub!
