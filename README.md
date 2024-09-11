# Gesture Volume Control

This project is a Python-based **Gesture Volume Control** system that utilizes **OpenCV**, **MediaPipe**, and **PyCaw**. It allows you to control your system's volume by detecting hand gestures through a webcam. By measuring the distance between your thumb and index finger, the system adjusts the volume accordingly.

## Table of Contents

1. [Introduction](#introduction)
2. [Environment Setup](#environment-setup)
3. [How It Works](#how-it-works)
4. [Running the Code](#running-the-code)
5. [Modules](#modules)
6. [Final Output](#final-output)

## Introduction

The **Gesture Volume Control** system leverages **OpenCV** and **MediaPipe** to detect hand gestures and adjust the system's volume in real-time. It calculates the distance between the thumb and index finger to determine whether to increase or decrease the volume. The visual feedback is provided through circles and lines on the video feed, along with a volume bar.

## Environment Setup

To run this project, you need to have Python installed. Follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/gesture-volume-control.git
    ```
2. Install the required dependencies:
    ```bash
    pip install opencv-python mediapipe pycaw
    ```
3. Ensure your webcam is functioning correctly.

## How It Works

- **Hand Detection**: Uses MediaPipe's Hands module to detect and track hand landmarks.
- **Distance Measurement**: Calculates the distance between the thumb and index finger to determine the volume adjustment.
- **Volume Control**: Adjusts the system's volume using PyCaw based on the detected distance.
- **Real-time Feedback**: Displays hand landmarks, volume adjustment indicators, and a volume bar directly on the video feed.

## Running the Code

1. Open the terminal and run the Python script:
    ```bash
    python main.py
    ```
2. The video feed will show hand landmarks and adjust the volume based on the thumb and index finger distance.
3. Ensure the input from the webcam is properly displayed.

## Modules

### HandTrackingModule

The `HandTrackingModule` is a custom module for detecting and tracking hand landmarks using MediaPipe. It includes functions to:
- Detect hands and draw landmarks
- Find the positions of key hand landmarks (e.g., thumb and index finger)

## Final Output

Here is an example of the final output, showing hand landmarks and volume control:

![Gesture Volume Control Output](https://github.com/mohamedelsayadd/Gesture-Volume-Control/blob/main/try.png)

