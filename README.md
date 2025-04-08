# Robust-Visual-Tracking-of-Drones-via-Integrated-Deep-Learning-and-ORB-Descriptors

This repository contains the inference module for our proposed drone detection and tracking framework, as introduced in our paper **"Robust Visual Tracking of Drones via Integrated Deep Learning and ORB Descriptors"**.

## Overview

The core functionality is implemented in `inferer_proposed.py`. This script integrates visual detection and tracking techniques to robustly identify and follow UAVs (drones) in complex environments. Our method combines YOLO-based LERFNet object detection with classical feature-based tracking (ORB) and custom strategies for re-detection when tracks are lost.

## Dataset

We use the [**DUT Anti-UAV**](https://github.com/wangdongdut/DUT-Anti-UAV) dataset for training and evaluation. This dataset provides a variety of challenging drone scenarios for benchmarking anti-UAV systems.

## Features

- Real-time UAV detection and tracking.
- ORB-based keypoint matching with ByteTrack for tracking after detection.
- Recovery from lost tracks via descriptor comparison.
- Easily integratable with other detection pipelines.

## Availability

⚠️ **The implementation in `inferer_proposed.py` will be released after the official publication of our paper.** Please stay tuned for updates.

## Requirements

- Python 3.8+
- OpenCV
- NumPy
- PyTorch (for YOLO)
- ByteTrack and LERFNet structures

## Usage

After the code is released, the module can be run as:

```bash
python inferer_proposed.py --weights path_to_yolo_weights.pt --source path_to_video
```

More instructions and configuration options will be provided upon release.

## Citation

If you find this work useful, please consider citing our paper:

**"Robust Visual Tracking of Drones via Integrated Deep Learning and ORB Descriptors"**  
*Citation details will be added after publication.*

## License

This project will be released under an open-source license after the paper is published.

---
