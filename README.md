# Lane Finder

The **Lane Finder** is a Python-based project that implements a lane detection algorithm similar to what Tesla uses in its autopilot system. It processes video frames to detect and highlight road lanes, making it a fundamental building block for autonomous driving systems.

## Features
- **Real-Time Lane Detection**: Processes video frames to detect lane lines in real-time.
- **Edge Detection**: Utilizes the Canny edge detection algorithm to find the edges of the lanes.
- **Region of Interest Masking**: Focuses on the area of the image most likely to contain lane lines.
- **Line Averaging**: Averages detected lines to produce stable and smooth lane boundaries.

## How It Works
- Captures frames from a video or camera feed.
- Detects edges using the Canny edge detection algorithm.
- Applies a region of interest mask to isolate relevant areas.
- Detects line segments using the Hough Transform and averages them to identify left and right lanes.
- Overlays detected lanes on the original video frame.

## Requirements
To run the project, ensure you have Python and the required libraries installed. Install the dependencies using:
```bash
pip install -r requirements.txt
```

## Steps to Run the Project

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/farhat-1203/Smart-Lane-Finder.git
    cd Smart-Lane-Finder
    ```

2. **Run the Lane Detection Script**:
    Execute the Python script to process the video:
    ```bash
    python3 main.py
    ```
    
## Project Structure
```
    lane-finder/
  ├── finding_lanes.py        # Main script for lane detection
  ├── requirements.txt        # List of dependencies
  ├── test2.mp4               # Sample video file for testing
  ├── LICENSE                 # License file
  └── README.md               # Project documentation

```
