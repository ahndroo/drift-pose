# Drift Angle Estimator

Real-time vehicle pose estimation and drift angle measurement using monocular vision.

## Overview

This project builds a vision-based pipeline that segments road boundaries, estimates vehicle pose frame-to-frame, and computes a continuous drift angle relative to the road centerline. No IMU, no GPS.

## Approach

- Lane and road boundary segmentation using [model]
- Frame-to-frame pose estimation via [optical flow / PnP solver]
- Road centerline extraction from segmentation mask
- Drift angle computed as delta between vehicle heading vector and centerline tangent
- (Bonus) 3D pose estimation using Depth Anything v2 for pitch and roll

## Dataset

[UPDATE]

## Results

[Add output video or GIF here]
[ADD QUALITATIVE RESULTS]

## Setup

```bash
git clone https://github.com/andrewkirk/drift-pose
cd drift-pose
pip install -r requirements.txt
```

[ADD DOCKER COMMANDS]

## Usage

```bash
python run.py --input path/to/video.mp4 --output output/
```

## Stack

- Python, PyTorch, OpenCV
- [Segmentation model]
- [Depth model]

## Notes


