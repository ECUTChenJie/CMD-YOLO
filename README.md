# CMD-YOLO

Official implementation of CMD-YOLO: A Synergistic Context Fusion and Semantic Calibration Network for Aerial Tiny Object Detection.

## Introduction

CMD-YOLO is a UAV-oriented aerial tiny object detection framework designed for remote sensing imagery with small object size, dense distributions, **large scale variation**, and complex background interference.  
To address these challenges, the proposed method introduces:

- MRF-CF: Multi-Receptive Field Context Fusion module for preserving fine-grained geometric details and local contextual information during downsampling.
- SCCAM: Semantic-Context Calibration Attention Module for improving contextual perception and suppressing background distraction in cluttered aerial scenes.
- ESD-Head: Enhanced Shallow Dense Detection Head spanning **P1-P5**, which enhances dense prediction and localization for tiny objects.

Extensive experiments on **VisDrone-2019** and **AITOD** demonstrate the effectiveness of CMD-YOLO for UAV tiny object detection.

---

## Highlights

- Designed for tiny object detection in UAV remote sensing imagery
- Multi-receptive-field context modeling for better feature retention
- Semantic-context calibration for complex aerial scenes
- Five-scale dense detection head for improved small-object localization
- Strong performance on VisDrone-2019 and AITOD

---

## Performance

### VisDrone-2019
- **mAP@0.5: 48.1%**
- +9.6 percentage points over the YOLO11s baseline

### AITOD
- mAP@0.5: 49.4%
- +4.6 percentage points over the YOLO11s baseline

---

## Repository Structure

```text
CMD-YOLO/
├── datasets/                # Dataset configuration files
├── models/                  # Network architecture definitions
├── ultralytics/             # Core framework / modified modules
├── weights/                 # Pretrained and trained weights
├── runs/                    # Training and evaluation outputs
├── train.py                 # Training script
├── val.py                   # Validation script
├── detect.py                # Inference script
├── requirements.txt         # Python dependencies
└── README.md
