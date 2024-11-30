# YOLOv5 Drunk Detection

This repository provides scripts and instructions for training the YOLOv5 model on a custom dataset. YOLOv5 is a state-of-the-art model for object detection tasks. Follow this guide to set up your dataset, configure training, and run the training process locally.

## Requirements

Ensure that the following software and libraries are installed before running the training:

- **Python 3.8+**
- **PyTorch 1.7+** (GPU support recommended for faster training)
- **CUDA** (required for GPU acceleration)
- **Git**
- **YOLOv5 repository** (this repository contains the training code and model)

## Installation

### Step 1: Install Dependencies

After cloning the repository, install the required dependencies by running the following command:

```bash
git clone pip install -U -r requirements.txt
```

### Step 2: Training the Model

Once your dataset is ready and data.yaml is configured, start the training process with the following command:

```bash
python train.py --img 640 --batch 16 --epochs 50 --data dataset/data.yaml --weights yolov5s.pt --cache
```
