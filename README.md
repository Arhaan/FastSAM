# Fast-SAM (Segment Anything Model)

## Overview

This project utilizes various image segmentation models to analyze and process images. The implemented code supports different segmentation models such as YOLO, SegFormer, Mask2Former, and DETR, allowing users to experiment with different segmentation techniques.

## Dependencies

Ensure you have the following dependencies installed before running the code:

- ultralytics
- transformers
- timm
- torch
- torchvision
- matplotlib
- requests
- PIL

You can install these dependencies using the following:

`pip install ultralytics transformers[torch] timm torch torchvision matplotlib requests Pillow`

## Usage

1. Open the Jupyter notebook `fastersam.ipynb` in a suitable environment (e.g., Google Colab).
2. Run the notebook cell by cell, making sure to install dependencies if prompted.
3. The notebook includes the ability to choose different segmentation models (`detr`, `mask2former`, `yolo`, `segformer`) and provides visualization of the segmented images.

## Models

- **DETR:** Facebook DETR ResNet-50 Panoptic segmentation model.
- **Mask2Former:** Facebook Mask2Former Swin Base COCO Panoptic segmentation model.
- **YOLO:** Ultralytics YOLOv8x segmentation model.
- **SegFormer:** NVIDIA SegFormer B1 Cityscapes 1024x1024 fine-tuned segmentation model.

## Functions

### `get_device()`

Returns the computing device (CPU).

### `model_provider(model)`

Provides the desired image segmentation model based on the specified model type.

### `find_bounding_box(data)`

Finds the bounding box of non-zero values in a 2D NumPy array.

### `show_masked_image(image, masks, bestseg)`

Displays a masked image with transparency.

## Author

Akshat Kumar Gupta (210050010), Arhaan Ahmad (210050016), Chaitanya Aggarwal (210050038), Hitesh Kumar (210050066), Yash Virani (210050170)

## Contact

For any inquiries, please contact [210050016[at]iitb.ac.in].



