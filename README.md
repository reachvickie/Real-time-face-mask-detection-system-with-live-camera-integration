# Real-time Face Mask Detection System 

## Overview

This repository contains a deep learning-based system for real-time face mask detection using live camera feed integration. The entire workflow is implemented within a **Jupyter Notebook**, making it easy to execute in environments like **Google Colab**.

The system uses an advanced object detection framework (YOLOv5) to quickly detect faces and classify them as **Mask** or **No Mask** in real-time.

---

## System Components and Methodology

The project workflow is encapsulated in a single Jupyter Notebook (`Face_Mask_Detection.ipynb`) and performs the following steps:

1. **Environment Setup**  
   - Mounts Google Drive for persistence.  
   - Clones the YOLOv5 repository to set up the detection framework.  

2. **Model Acquisition**  
   - Downloads or loads a pre-trained face mask detection model (e.g., `runs/train/exp/weights/last.pt`).  

3. **Real-Time Integration**  
   - Uses Google Colab’s native camera functions and OpenCV to capture frames from the webcam.  

4. **Inference**  
   - YOLOv5 performs real-time object detection on each frame to locate faces and classify them as **Mask** or **No Mask**.  

5. **Visualization**  
   - Displays bounding boxes and class labels directly in the notebook output for easy visualization.

---

## Installation and Setup

This project is designed to run primarily in **Google Colab**.

### Prerequisites

- A **Google Account** (to access Colab).  
- A **working webcam** (for live detection).  

### Running the Project

1. **Upload**  
   - Upload the `Face_Mask_Detection.ipynb` notebook file to your Google Drive.  

2. **Open in Colab**  
   - Open the notebook in Google Colab.  

3. **Run Cells**  
   - Execute all cells sequentially. Initial cells handle dependency installation and repository cloning.  

4. **Grant Camera Access**  
   - When prompted, allow the notebook to access your webcam to start real-time detection.  

---

## Dependencies

The primary libraries and tools used in this project include:

- **YOLOv5 Framework** (cloned from GitHub)  
- **PyTorch** (underlying YOLOv5 framework)  
- **OpenCV (cv2)**  
- **NumPy**  
- **google.colab** (for camera and drive functions)  

---

## Usage

- Execute all notebook cells in order.  
- The notebook will automatically start capturing frames from your webcam and perform real-time mask detection.  
- Detected faces will be highlighted with bounding boxes and labeled as **Mask** or **No Mask**.  

---

## License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- [YOLOv5](https://github.com/ultralytics/yolov5) for the object detection framework.  
- OpenCV and PyTorch communities for support and resources.  
