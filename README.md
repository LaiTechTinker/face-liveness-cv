# Face Recognition Practice Project

A practice computer vision project for exploring face detection and liveness-related signals in video. The experiments are organized as Jupyter notebooks and use MediaPipe, OpenCV, NumPy, and Matplotlib.

## Features

- Open and inspect video files
- Extract and resize video frames
- Detect faces and face keypoints
- Detect facial landmarks
- Measure mouth opening and eye-aspect ratio
- Process video samples over time

## Project Files

- `face_liveness_detection.ipynb` - Video loading, frame extraction, and frame sampling
- `face_detectionphase3.ipynb` - Image and video face detection with MediaPipe
- `facial_landmarks.ipynb` - Facial landmarks and mouth measurements
- `building_mouth_opening.ipynb` - Time-based eye and mouth measurements
- `small_videosampling_pipeline.ipynb` - Frame sampling and Base64 encoding
- `test_video.mp4` - Sample video used by the notebooks
- `blaze_face_short_range.tflite` - MediaPipe face detector model
- `face_landmarker.task` - MediaPipe face landmarker model

## Requirements

- Python 3.9 or newer
- Jupyter Notebook or JupyterLab

The current dependency list is in `requirements.txt`.

## Setup

From the project directory, create and activate a virtual environment:

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

Install the project dependencies and Jupyter:

```powershell
pip install -r requirements.txt
pip install opencv-python jupyter
```

## Run

Start Jupyter from the project directory:

```powershell
jupyter notebook
```

Open a notebook and run the cells from top to bottom. Keep `test_video.mp4` and the model files in the project directory unless you update the paths in the notebook.

## Notes

- Use your own consented video data for additional testing.
- This is a learning and experimentation project, not a production-ready identity or liveness system.