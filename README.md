# Udacity Dog Image Classifier

Python image classification project comparing ResNet, AlexNet, and VGG using pre-trained CNN models. Built to evaluate dog detection, breed classification accuracy, and model runtime.

# Project Overview

This project was completed as part of the Udacity AWS AI Programming learning track.

The goal of the project is to use Python with pre-trained convolutional neural network (CNN) models to classify pet images and compare the performance of three different architectures:

- ResNet
- AlexNet
- VGG

The project focuses on using Python to process image data, organize classification results, calculate accuracy statistics, and compare model performance.

# Objectives

The main objectives of this project were to:

1. Correctly identify which images contain dogs and which do not.
2. Correctly identify the breed of dog in images that contain dogs.
3. Compare the performance of ResNet, AlexNet, and VGG.
4. Compare model accuracy with execution time to determine the best overall model.

# Technologies Used

- Python
- PyTorch
- Convolutional Neural Networks
- Pre-trained ImageNet models
- argparse
- Python dictionaries and lists
- File handling
- Bash scripting

# Project Structure

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
```

# How the Program Works

The program follows this workflow:

1. Reads command-line arguments.
2. Extracts pet labels from image filenames.
3. Uses a pre-trained CNN model to classify each image.
4. Compares the classifier prediction with the actual pet label.
5. Determines whether each label represents a dog or a non-dog.
6. Calculates classification statistics.
7. Prints the final results.
8. Compares the performance of all three CNN architectures.

# Running the Project

Run the program with:

python check_images.py --dir pet_images/ --arch vgg --dogfile dognames.txt

# Available model architectures:
resnet
alexnet
vgg

# Example:
python check_images.py --dir pet_images/ --arch resnet --dogfile dognames.txt

# Running All Models

To run all three CNN architectures automatically:

sh run_models_batch.sh

This produces:
resnet_pet-images.txt
alexnet_pet-images.txt
vgg_pet-images.txt

# Model Results
| Model   | Dogs Correct | Non-Dogs Correct | Breeds Correct | Overall Label Match |
| ------- | -----------: | ---------------: | -------------: | ------------------: |
| ResNet  |       100.0% |            90.0% |          90.0% |               82.5% |
| AlexNet |       100.0% |           100.0% |          80.0% |               75.0% |
| VGG     |       100.0% |           100.0% |          93.3% |               87.5% |


# Best Performing Model

VGG produced the strongest overall results.

It achieved:

100% accuracy identifying dog images

100% accuracy identifying non-dog images

93.3% accuracy identifying dog breeds

87.5% overall label match accuracy

Although VGG required more execution time than ResNet and AlexNet, it provided the best overall accuracy for the main project objectives.

# Custom Image Testing

The completed program was also tested using four uploaded images:

Golden Retriever
Rotated Golden Retriever
Cat
Coffee Mug

ResNet and VGG correctly recognized both dog images as Golden Retrievers and correctly identified the cat and coffee mug as non-dogs.

AlexNet correctly classified the original dog image but classified the rotated image as a Cocker Spaniel.

This demonstrates how image orientation can affect model predictions.

# Key Skills Demonstrated

This project demonstrates experience with:

Python programming

Working with pre-trained machine learning models

Image classification

Data structures

Functions

File processing

Command-line interfaces

Model evaluation

Accuracy metrics

Runtime comparison

Bash scripting

Debugging Python programs

# Final Conclusion

VGG was the best CNN model architecture for the main project because it correctly classified dogs and non-dogs with 100% accuracy and achieved the highest dog-breed classification accuracy at 93.3%.

ResNet provided a strong alternative because it completed classification much faster while still achieving 90% breed accuracy.

# Author

Mafeyisopin Ayeni

GitHub: mafeyisopin629-spec

# Acknowledgements

This project was completed as part of the Udacity AWS AI Programming curriculum.

The image classifier and pre-trained CNN architectures used in this project were provided as part of the Udacity project environment.
