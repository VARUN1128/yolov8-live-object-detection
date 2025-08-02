
---

## 📄 `README.md`

````markdown
# 🧠 YOLOv8 Live Object Detection

This repository provides a Python implementation for **real-time object detection** using [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics) and OpenCV. The script captures webcam input, detects objects frame-by-frame, draws bounding boxes and labels, and saves the annotated output as a video.

## 📸 Example

![demo](https://github.com/ultralytics/assets/raw/main/yolov8/assets/banner_yolov8.png)

---

## 🧰 Features

- Real-time object detection with `YOLOv8`
- Uses webcam or can be modified for video input
- Displays live object detection with bounding boxes and confidence scores
- Saves processed video to `output.avi`
- Custom class name labeling

---

## 📦 Requirements

- Python 3.7+
- [Ultralytics](https://pypi.org/project/ultralytics/)
- [OpenCV](https://pypi.org/project/opencv-python/)

### Install via pip:

```bash
pip install ultralytics opencv-python
````

---

## 🚀 How to Run

### 1. Clone this repository

```bash
git clone https://github.com/your-username/yolov8-live-object-detection.git
cd yolov8-live-object-detection
```

### 2. Download YOLOv8 Weights

Download `yolov8n.pt` (or another version like `yolov8s.pt`) from:
👉 [https://github.com/ultralytics/ultralytics/releases](https://github.com/ultralytics/ultralytics/releases)

Place it inside the `YOLO-Weights/` folder or update the path in the code.

### 3. Run the Script

```bash
python yolo_webcam.py
```

> Press `1` to exit the live feed.

---

## 🧠 How It Works

* Loads YOLOv8 model using Ultralytics API.
* Captures frames from the webcam.
* Performs object detection using `model(img, stream=True)`.
* Draws bounding boxes and confidence labels using OpenCV.
* Saves output to `output.avi`.

---

## 📁 Project Structure

```
.
├── yolo_webcam.py              # Main detection script
├── YOLO-Weights/
│   └── yolov8n.pt              # YOLOv8 model weights
├── output.avi                  # Output video (generated after run)
└── README.md                   # Project documentation
```

---

## ✏️ Customization

* **Use video file** instead of webcam:

  ```python
  cap = cv2.VideoCapture('your_video.mp4')
  ```
* **Change model**:
  Replace with `yolov8s.pt`, `yolov8m.pt`, etc.
* **Modify frame rate or resolution** by adjusting:

  ```python
  out = cv2.VideoWriter(..., 10, (frame_width, frame_height))
  ```

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙌 Acknowledgements

* [Ultralytics](https://github.com/ultralytics/ultralytics)
* [OpenCV](https://opencv.org/)

---

## 🔗 Connect

For suggestions or collaborations, feel free to raise an issue or PR!

```

---

Would you like:
- A sample `requirements.txt`?
- To convert this into a pip-installable package?
- Or help making a `.py` version of the class-based version for scalability?

Let me know how you plan to evolve this project!
```
