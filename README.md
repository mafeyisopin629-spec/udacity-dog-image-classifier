# Udacity Dog Image Classifier

Python image classification project comparing ResNet, AlexNet, and VGG using pre-trained CNN models. Built to evaluate dog detection, breed classification accuracy, and model runtime.

## Project Overview

This project was completed as part of the Udacity AWS AI Programming learning track.

The goal of the project is to use Python with pre-trained convolutional neural network (CNN) models to classify pet images and compare the performance of three different architectures:

- ResNet
- AlexNet
- VGG

The project focuses on using Python to process image data, organize classification results, calculate accuracy statistics, and compare model performance.

## Objectives

The main objectives of this project were to:

1. Correctly identify which images contain dogs and which do not.
2. Correctly identify the breed of dog in images that contain dogs.
3. Compare the performance of ResNet, AlexNet, and VGG.
4. Compare model accuracy with execution time to determine the best overall model.

## Technologies Used

- Python
- PyTorch
- Convolutional Neural Networks
- Pre-trained ImageNet models
- argparse
- Python dictionaries and lists
- File handling
- Bash scripting

## Project Structure

```text
.
├── check_images.py
├── get_input_args.py
├── get_pet_labels.py
├── classify_images.py
├── adjust_results4_isadog.py
├── calculates_results_stats.py
├── print_results.py
├── classifier.py
├── dognames.txt
├── imagenet1000_clsid_to_human.txt
├── run_models_batch.sh
├── run_models_batch_uploaded.sh
├── pet_images/
├── uploaded_images/
├── resnet_pet-images.txt
├── alexnet_pet-images.txt
└── vgg_pet-images.txt
