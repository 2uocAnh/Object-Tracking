# Background Subtraction for Object Tracking

This repository contains implementations of **Background Subtraction** — a technique used to separate foreground objects from the background in video sequences.

### Overview
Background Subtraction is a widely used method in the fields of image processing and video analysis. It is especially helpful for tasks such as:
- **Object Tracking**
- **Motion Detection**
- **Segmentation**

By isolating moving objects from a stationary background, this method allows for better analysis and understanding of dynamic scenes in video footage.

### Key Features
- **Object Detection**: Identifies moving objects in video sequences.
- **Object Tracking**: Uses Euclidean distance to assign unique IDs to objects and track them over time.
- **Real-Time Processing**: The method can process video streams in real time.

### How It Works
1. **Background Subtraction**: The algorithm applies a background subtraction technique (e.g., `BackgroundSubtractorMOG2`) to separate the moving objects from the static background.
2. **Object Detection**: Contours are found in the foreground mask to identify regions of interest (RoI) where objects are located.
3. **Object Tracking**: A custom tracking algorithm (Euclidean Distance Tracker) assigns a unique ID to each detected object and tracks it through successive frames.
4. **Display**: Bounding boxes are drawn around the detected objects, and their IDs are displayed.
