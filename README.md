# NBA-GOATS-Image-Classification

## Overview

This project was created as a way to learn PyTorch and explore image classification. I chose to focus on a few NBA players, since I enjoy following the NBA.

Before starting, I had a basic understanding of neural networks — that they are an efficient way to label and predict complex data using gradient descent, a learning rate, and activation functions. However, applying these concepts in code taught me much more about how they actually work in practice.

## Project Structure
├── nba_classifier.ipynb   # Main Colab notebook
├── README.md
└── /data  

## Getting Started

This project runs entirely in Google Colab — no local installation required.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](YOUR_COLAB_LINK_HERE)

### Requirements
The following libraries are used and can be installed directly in the notebook:

- Python 3.x (via Colab)
- PyTorch + torchvision
- bing-image-downloader
- matplotlib
- numpy

To install any missing dependencies within the notebook:
\```python
!pip install bing-image-downloader
\```

## What I Learned

* Throughout this project, I learned to:

* Use PyTorch’s ImageFolder and DataLoader modules to organize data into training, testing, and validation sets.

* Utilize a GPU to significantly speed up training time.

* Create a neural network specialized for image classification.

* Compare my model with a pre-trained model.

* Compare true vs. predicted results to evaluate model performance.

* Work with AI tools (mainly Claude) to assist with debugging and implementation — while always verifying the AI-generated code before using it.

## Dataset

* I collected images using the bing_image_downloader library. While it was quick and easy to use, I discovered that the results were prone to inaccuracies.

* For example, an image of actor Michael B. Jordan was downloaded instead of basketball player Michael Jordan, given my search term "Michael Jordan". I manually removed this and other images including other inaccuracies, but I understand that this isn’t a sustainable solution for larger or production-level projects. In such cases, for accurate search terms, like "Michael Jordan NBA" or "Michael Jeffrey Jordan" might prove more useful, or using a different package to download images.

## Results
The custom CNN achieved ~88% test accuracy.  
The pre-trained model (e.g. ResNet18) achieved 90% test accuracy.


## Future Improvements

* Use a more reliable data collection method to ensure accurate labeling.

* Expand the dataset to include more representative and diverse examples.

* Experiment with different architectures or data augmentation techniques to improve model accuracy.

## Purpose

* This project is intended for educational purposes. My goal was to better understand how image classification works in PyTorch, and I hope others can also learn something from it along the way. Feel free to use the project. For any inquiries, please reach out to my email or Medium blog post.

## Sources of inspiration

ImageNet Classification with Deep Convolutional Neural Networks
https://proceedings.neurips.cc/paper_files/paper/2012/file/c399862d3b9d6b76c8436e924a68c45b-Paper.pdf

Build Your First PyTorch Model (Linear Regression)  
https://www.youtube.com/watch?v=QPCFnbonpNQ&t=226s

Build Your First Pytorch Model In Minutes! [Tutorial + Code]  
https://www.youtube.com/watch?v=tHL5STNJKag&t=931s
