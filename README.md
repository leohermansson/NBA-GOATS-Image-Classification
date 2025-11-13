# NBA-GOATS-Image-Classification

## Overview

This project was created as a way to learn PyTorch and explore image classification. I chose to focus on a few NBA players, since I enjoy following the NBA.

Before starting, I had a basic understanding of neural networks — that they are an efficient way to label and predict complex data using gradient descent, a learning rate, and activation functions. However, applying these concepts in code taught me much more about how they actually work in practice.

## What I Learned

Throughout this project, I learned to:

Use PyTorch’s ImageFolder and DataLoader modules to organize data into training, testing, and validation sets.

Utilize a GPU to significantly speed up training time.

Compare true vs. predicted results to evaluate model performance.

Work with AI tools (mainly Claude) to assist with debugging and implementation.

## Dataset

I collected images using the bing_image_downloader library. While it was quick and easy to use, I discovered that the results were sometimes inaccurate.

For example, an image of actor Michael B. Jordan was downloaded instead of basketball player Michael Jordan. I manually removed this and three other incorrect images, but I understand that this isn’t a sustainable solution for larger or production-level projects.

In total, I used 246 images:

Most classes had 50 images

Two classes had 48 images due to inconsistencies in the downloaded data

## Future Improvements

There’s plenty of room for improvement:

Use a more reliable data collection method to ensure accurate labeling.

Expand the dataset to include more representative and diverse examples.

Experiment with different architectures or data augmentation techniques to improve model accuracy.

## Purpose

This project is intended for educational purposes only. My goal was to better understand how image classification works in PyTorch, and I hope others can also learn something from it along the way.
