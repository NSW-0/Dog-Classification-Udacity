# Dog-Classification-Udacity
Image Classification and Results Evaluation for Pet Images
This project implements a system for classifying pet images using pretrained CNN (Convolutional Neural Network) models. The objective is to assess the performance of different CNN architectures in accurately classifying pet images based on their filenames. Each image is classified into specific categories, and the program then compares the classifier's predictions with the true identity of the pet, which is encoded in the image's filename. The project evaluates how well the model performs in terms of both correct classification and breed identification.

Key Components:

Command Line Interface (CLI):

The program accepts command-line inputs using argparse. Users specify the directory containing pet images, the CNN model architecture to use (resnet, alexnet, vgg), and a text file with dog breed names. If any argument is missing, default values are used.

Image Label Extraction:

The pet image labels are extracted from the filenames. These labels are compared against the results of the classifier function to evaluate the model's performance.

Image Classification:

Using a pretrained CNN model (selected by the user via the command-line arguments), the program classifies the pet images. It then compares these predicted labels with the true pet labels derived from the filenames.

Results Comparison:

The classifier’s results are compared to the true labels to determine whether the classification was correct, and whether the correct breed was identified. Misclassifications are tracked for both dog/non-dog labels and breed-specific labels.

Results Evaluation:

The project calculates various statistics based on the results:

Total number of images processed

Number of dog and non-dog images

Number of correct matches between pet and classifier labels

Number of correctly classified dogs and non-dogs

Percentage of correctly classified dogs, breeds, and matches

Summary Output:

After processing the images, a summary of the classification results is printed, which includes counts and percentages for each statistic. Additionally, users can choose to print misclassified dog images or incorrect breed classifications for further analysis.

Features:

Model Flexibility: Supports three CNN models (resnet, alexnet, vgg) for image classification.

Error Analysis: Optionally print details of misclassified dogs and breeds.

Performance Metrics: Provides detailed performance statistics, including accuracy for both dog classification and breed recognition.
