# GatiSense: Real-Time Traffic Density Estimation

GatiSense is a computer vision project that utilizes a fine-tuned YOLOv8 model to perform real-time traffic analysis from a video feed. It detects vehicles, counts them in designated lanes, and classifies the traffic density as "Heavy" or "Smooth".

## Features

- **Real-time Vehicle Detection**: Employs a YOLOv8 model to accurately detect vehicles in video streams.
- **Lane-Specific Counting**: Isolates and counts vehicles in two distinct lanes using predefined regions of interest.
- **Traffic Density Estimation**: Classifies the traffic flow in each lane as "Heavy" or "Smooth" based on vehicle counts.
- **Output Visualization**: Generates a processed video file with bounding boxes around detected vehicles, along with on-screen text displaying vehicle counts and traffic density for each lane.

## How It Works

The core logic is in the [`real_time_traffic_analysis.py`](YOLOv8_Traffic_Density_Estimation-master/real_time_traffic_analysis.py) script.

1.  **Model Loading**: A pre-trained YOLOv8 model from [`models/best.pt`](YOLOv8_Traffic_Density_Estimation-master/models/best.pt) is loaded.
2.  **Video Processing**: The script reads the input video (`sample_video.mp4`) frame by frame.
3.  **Region of Interest (ROI)**: Two quadrilateral regions are defined to represent the left and right lanes, focusing the detection process on these specific areas.
4.  **Object Detection**: Each frame is passed to the YOLOv8 model, which returns the bounding boxes of detected vehicles.
5.  **Counting & Classification**:
    -   Vehicles are assigned to the left or right lane based on the center of their bounding box.
    -   The number of vehicles in each lane is counted.
    -   The traffic density for each lane is classified as "Heavy" or "Smooth" by comparing the count to the `heavy_traffic_threshold`.
6.  **Output Generation**: The script annotates the video frames with bounding boxes, vehicle counts, and density status. The resulting video is displayed on the screen and saved as `processed_sample_video.avi`.

## Project Structure
