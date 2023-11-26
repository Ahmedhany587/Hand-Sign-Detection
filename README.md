# Hand-Sign-Detection



## Table of Contents
1. [Introduction](#introduction)
2. [Dependencies](#dependencies)
3. [Image Collection](#image-collection)
4. [Image Labelling](#image-labelling)
5. [Data Preparation](#data-preparation)
6. [Model Training](#model-training)
7. [Model Evaluation](#model-evaluation)
8. [Inference](#inference)
9. [Real-Time Inference](#real-time-inference)
10. [Freezing the Graph](#freezing-the-graph)
11. [Conversion to TFJS](#conversion-to-tfjs)
12. [Conversion to TFLite](#conversion-to-tflite)

## 1. Introduction
This project involves creating an object detection model using TensorFlow. The pipeline includes collecting images, labelling them, preparing the data, training the model, and deploying it for real-time inference. The process covers both single image detection and real-time detection from a webcam feed.



## 3. Image Collection
Images are collected for specified labels using the OpenCV library. Ensure that the necessary folders are set up before running the image collection script.

## 4. Image Labelling
LabelImg is used for labelling images. Follow the installation instructions for LabelImg provided in the script.

## 5. Data Preparation
TFRecords are generated from the labelled images using the `generate_tfrecord.py` script. Make sure to have the required script and dependencies installed.

## 6. Model Training
The project uses a pre-trained model from the TensorFlow Model Zoo for transfer learning. The model is trained using the `model_main_tf2.py` script.

## 7. Model Evaluation
Evaluate the trained model using the same `model_main_tf2.py` script with evaluation parameters.

## 8. Inference
Load the trained model and perform inference on a single image using the provided script.

## 9. Real-Time Inference
Run the real-time inference script to detect objects in the webcam feed. Ensure the webcam is properly connected.

## 10. Freezing the Graph
Freeze the trained model's graph for deployment using the `exporter_main_v2.py` script.

## 11. Conversion to TFJS
Convert the frozen graph to TensorFlow.js format using the `tensorflowjs_converter` tool.

## 12. Conversion to TFLite
Convert the frozen graph to TensorFlow Lite format using the provided scripts.

**Note**: Make sure to adjust paths and configurations according to your project structure and requirements.
