**Stereo Vision-Based Object Detection using YOLOv8**

This project uses stereo vision (two cameras) and YOLOv8 to detect objects (bottle in this case), estimate their 3D position, and calculate their distance & depth.

**Features**

Stereo Vision: Uses two cameras to capture frames.

YOLOv8 Object Detection: Detects objects in real-time.

3D Position Calculation: Estimates object location & height.

Multi-Threading: Efficient frame capturing for smooth processing.

Real-Time Visualization: Displays bounding boxes & distance values.

**Requirements**

Ensure you have the following installed before running the project:

pip install opencv-python numpy torch ultralytics

**How It Works?**

Captures frames from two cameras simultaneously.

Uses YOLOv8 to detect objects in each frame.

Calculates disparity between left & right camera views.

Computes depth & distance using the stereo vision formula:
Z = (Baseline * Focal length)/Disparity

Displays bounding boxes with real-time distance & depth calculations

