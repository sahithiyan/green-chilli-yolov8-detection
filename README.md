
# Green Chilli YOLOv8 Detection

This repository contains a YOLOv8 model trained to detect green chillies. 

## Project Overview

This project demonstrates the training and deployment of a YOLOv8 nano model for object detection. The model is trained on a custom dataset of green chillies, aiming to identify them in images.

## Dataset

The dataset used for training, validation, and testing consists of images of green chillies. It is split into training, validation, and test sets.

## Model Training

The YOLOv8n model was trained for 80 epochs with early stopping. Key training parameters:

*   **Model:** `yolov8n.pt` (pretrained COCO weights)
*   **Data:** `/content/dataset/data.yaml`
*   **Epochs:** 80
*   **Image Size:** 416
*   **Batch Size:** 16
*   **Patience:** 20 (for early stopping)

## Evaluation Metrics

After training, the model achieved the following performance metrics:

*   **mAP50:** 0.911
*   **mAP50-95:** 0.689
*   **Precision:** 0.928
*   **Recall:** 0.9

## Prediction Examples

Sample predictions on the test set are available in the `runs/detect/test_predictions` directory.

## Weights

The best trained model weights are saved as `best_green_chilli.pt`.

