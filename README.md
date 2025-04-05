# ByteTrack

A simplified implementation of the ByteTrack algorithm for object tracking using IoU-based association. This project was completed as part of the CSI4533 university class.

## 🔍 Overview

This implementation tracks objects across video frames from the vivaFF database using a simplified version of the ByteTrack algorithm. Performance is evaluated using the ID-switch metric.

![Object Tracking Demo](./tracking_video.gif)

## 🧠 Algorithm Specifications

- Use IoU (Intersection over Union) for detection association
- Motion prediction based on center displacement (dx, dy)
- Tracklets are terminated after 20 frames without association
- Only tracklets with 50+ detections are included in final results

## 📊 Key Features

- Filters detections with confidence scores ≥ 0.5
- Visualizes object tracks with unique ID colors
- Generates JSON output for evaluation
- Creates demo video of tracking results

## 🚀 Usage

1. Clone this repository
2. Run in Google Colab or local Python environment
3. Set parameters as needed in config section
4. Execute notebook to perform tracking
5. View generated video and tracking metrics
   
## 🎬 Demo

You can view a demonstration of our tracking implementation below:

https://user-images.githubusercontent.com/12345678/tracking_video.mp4

## ⚙️ Requirements

- Python 3.7+
- OpenCV
- NumPy
- JSON

## 📁 Project Structure

```
.
├── notebook.ipynb       # Main implementation notebook
├── output.json          # Generated tracking results
├── tracking_result.mp4  # Demo video
└── README.md            # This file
```
---
## 👥 Authors

- **Bruno Kazadi**
