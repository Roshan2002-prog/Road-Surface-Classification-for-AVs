# Road-Surface-Classification-for-AVs
This project focuses completely on different types of road surfaces classification like ice, snow, asphalt and concrete cracks using CNNs  Resources  Readme
This project focuses completely on different types of road surfaces classification like ice, snow, asphalt and concrete cracks using CNNs This project implements a deep learning pipeline for automated road surface classification using the EfficientNetV2-M architecture, robust data augmentation with Albumentations, and thorough benchmarking on the RSCD dataset. The pipeline is optimized for real-world scenarios relevant to autonomous vehicles and intelligent transportation.

Features Classification of 27 diverse road surface classes (e.g., wet/dry asphalt, mud, snow, ice, concrete, etc.)

Advanced data augmentation: Random Rain, Snow, Shadow, Brightness/Contrast, Motion Blur, Horizontal Flip, and combinations thereof

Comparison of multiple architectures: EfficientNetV2-M (primary), ResNet-50, ConvNeXt Base

Training acceleration and scalability on NVIDIA DGX

Ready-to-use code for visualization of augmented images

Detailed result analysis, including confusion matrix and per-class metrics

Example Augmentations The repository includes scripts to generate visual summaries of multiple augmentations in a grid (see /AUGMENTATION_2x4.png for an example).

Getting Started Prerequisites

Python 3.8+

Albumentations

PyTorch

OpenCV (cv2)

tqdm

Matplotlib

NumPy

Prepare your images: Place your target image(s) in the repo folder (e.g. Crack_Image.jpeg).

Run augmentation visualization: Use the provided scripts (see augmentations_grid.py) to generate a grid of all augmented versions for report or analysis.

Model Training and Evaluation: Follow the main notebook/script to train EfficientNetV2-M (or a baseline model) and evaluate against the RSCD or your dataset.

Results: Confusion matrix and example predictions will be saved to disk
