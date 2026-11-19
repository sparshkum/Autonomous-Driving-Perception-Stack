
# Autonomous Driving Perception Stack

## 1. Project Overview

This project implements a computer vision-based
autonomous driving perception pipeline.

The system processes driving video frames to detect
objects, track their movement, identify lane markings,
and estimate relative depth.

## 2. Technologies Used

- Python
- YOLO11
- OpenCV
- ByteTrack
- MiDaS
- ONNX
- PyTorch
- Google Colab

## 3. Main Features

1. Object detection using YOLO11.
2. Multi-object tracking using ByteTrack.
3. Lane detection using OpenCV.
4. Monocular relative depth estimation using MiDaS.
5. Integrated perception visualization.
6. Processing time and FPS evaluation.
7. YOLO model export to ONNX.

## 4. System Architecture

Driving Video Input
        |
        v
YOLO Object Detection
        |
        v
ByteTrack Object Tracking

Driving Frames
        |
        v
OpenCV Lane Detection

Driving Frames
        |
        v
MiDaS Depth Estimation

        |
        v
Integrated Perception Output

## 5. Experimental Results

- Total frames processed: 62
- Average processing time: 29.34 ms
- Average processing FPS: 34.08
- Input video FPS: 30
- Resolution: 640 x 360

## 6. Dataset

A sample traffic video was used for the
initial pipeline demonstration.

BDD100K/KITTI fine-tuning is not claimed
as completed in this prototype.

## 7. Limitations

- Depth estimation provides relative depth,
  not calibrated distance in metres.
- Classical lane detection may be affected
  by lighting and road conditions.
- The system is a perception prototype,
  not a road-ready autonomous vehicle.

## 8. Future Scope

- CARLA simulator integration.
- ROS2 camera streaming.
- TensorRT optimization.
- Lane segmentation models.
- Dataset-based detection evaluation.

## 9. Project Outputs

Refer to the outputs, models and results folders.

## 10. Disclaimer

This project is developed for educational
and experimental purposes.
