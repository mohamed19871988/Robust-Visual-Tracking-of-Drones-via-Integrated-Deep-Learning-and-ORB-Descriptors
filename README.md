# Robust-Visual-Tracking-of-Drones-via-Integrated-Deep-Learning-and-ORB-Descriptors
Drone Detection and Tracking Inference Module
This repository contains the inference module for our proposed drone detection and tracking framework, as introduced in our upcoming research paper. The core functionality is implemented in inferer_proposed.py.

Overview
The module provides an integrated approach to detect and track UAVs (drones) using a combination of deep learning detection (YOLO-based LERFNet) and classical tracking techniques (ByteTrack, ORB features). The proposed method aims to enhance performance in complex environments with robust matching and re-detection strategies.

Dataset
We use the DUT Anti-UAV dataset for training and evaluation. This dataset provides a variety of challenging drone scenarios for benchmarking anti-UAV systems.

Features
Real-time inference for drone detection.

Efficient tracking using ORB descriptors and keypoint matching.

Mechanism for handling lost tracks and re-identification.

Designed for modular integration with detection pipelines.

Availability
⚠️ The main class and method implementations in inferer_proposed.py are currently withheld and will be made publicly available after the official publication of our paper. Stay tuned for updates!

Requirements
Python 3.8+

OpenCV

NumPy

PyTorch (for YOLO detection)

Other dependencies as required for the detection framework

Usage
After the code is released:

python inferer_proposed.py --weights path_to_weights.pt --source path_to_video

Citation
If you use this work in your research, please cite our paper once it is published (citation details will be added here post-publication).

License
This project will be released under an open-source license after publication.
