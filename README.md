# NBA GOATS Image Classification


## Overview

This project was created as a way to learn PyTorch and explore image classification. I chose to focus on a few NBA players, since I enjoy following the NBA.

Before starting, I had a basic understanding of neural networks — that they are an efficient way to label and predict complex data using gradient descent, a learning rate, and activation functions. However, applying these concepts in code taught me much more about how they actually work in practice.

## Project Structure
├── nba_classifier.ipynb   # Main Colab notebook
├── README.md
└── /data                  # Image folders (not committed to repo)

## Getting Started

This project runs entirely in Google Colab — no local installation required.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1JaFR53X_9cjXHuJt3l1X6Qf5mzXk3-Mi#scrollTo=hUii2ygs4JkA)

How do I know which versions of the packages I have? I didn't check when i did the project.
### Requirements
The following libraries are used and can be installed directly in the notebook:

- Python: 3.12.13 (via Colab)
- PyTorch(torchvision): 0.25
- bing-image-downloader: 1.1.2
- seaborn: 0.13.2
- matplotlib: 3.10.0
- numpy: 2.0.2

## What I Learned

Throughout this project, I learned to:

- Use PyTorch's ImageFolder and DataLoader to organize data into training, validation, and test sets.
- Use a GPU to significantly speed up training.
- Build a CNN specialized for image classification.
- Compare my model against a pre-trained ResNet18 baseline.
- Evaluate performance by visualizing true vs. predicted labels.
- Use AI tools (mainly Claude) to assist with debugging — while always verifying generated code before using it.

## Dataset

Images were collected using the `bing_image_downloader` library. While quick to use, the results were prone to inaccuracies — for example, searching "Michael Jordan" returned images of actor Michael B. Jordan. I manually cleaned these, but this doesn't scale to larger projects. More specific search terms like "Michael Jordan NBA" or a more robust scraping library would be better alternatives.

## Results
The custom CNN achieved ~88% test accuracy.  
The pre-trained model (e.g. ResNet18) achieved 90% test accuracy.


## Future Improvements

* Use a more reliable data collection method to ensure accurate labeling.

* Expand the dataset to include more representative and diverse examples.

* Experiment with different architectures or data augmentation techniques to improve model accuracy.

## Purpose

* This project is intended for educational purposes. My goal was to better understand how image classification works in PyTorch, and I hope others can also learn something from it along the way. Feel free to use the project. For any inquiries, please reach out to my email or Medium.

Mail: leo.hermansson@gmail.com
Medium: I Trained a Neural Network to Recognize NBA Legends
https://medium.com/@leo.hermansson/i-trained-a-neural-network-to-recognize-nba-legends-ee5cd6e1e786

## Sources of inspiration

ImageNet Classification with Deep Convolutional Neural Networks
https://proceedings.neurips.cc/paper_files/paper/2012/file/c399862d3b9d6b76c8436e924a68c45b-Paper.pdf

Build Your First PyTorch Model (Linear Regression)  
https://www.youtube.com/watch?v=QPCFnbonpNQ&t=226s

Build Your First Pytorch Model In Minutes! [Tutorial + Code]  
https://www.youtube.com/watch?v=tHL5STNJKag&t=931s
