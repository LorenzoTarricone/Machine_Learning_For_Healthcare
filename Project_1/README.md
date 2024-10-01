 
# PROJECT 1

## Group components:
Sophia Houhamdi, Eva Sarlin, Lorenzo Tarricone


## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [File Structure](#file-structure)

## Introduction

Project 1 focuses on interpretable and explainable classification for medical data using machine-learning methods. It consists of three parts: 
1. The first part involves tabular data analysis, specifically using the Kaggle Heart Failure Prediction Dataset, to explore features, handle data pitfalls, and implement interpretable models like Logistic Lasso Regression.
2. The second part deals with imaging data analysis, utilizing the Kaggle Chest X-Ray Images (Pneumonia) dataset. It includes tasks such as CNN classification, Integrated Gradients, and Grad-CAM for interpretability.
3. The third part involves summarizing findings, answering general questions about the methods used, and exploring techniques for interpretable classification with shallow and deep machine-learning models. The goal is to gain insights beyond predictive performance by understanding feature importance and model interpretability.

## Features

In our implementation we finetuned a pretrained ResNet (adapting from [here](https://www.kaggle.com/code/teyang/pneumonia-detection-resnets-pytorch))

## Installation

A `requirement.txt` file is provided containig all the packages we used for this project. In order to install them you can simply run. To ensure they are all installed in your current environment please run

`pip install -r requirements.txt`

## Usage

Once you have all the needed packages in your envuroment as described above, you can simply open the notebook correponding to the section you are interested in and run the code smoothly.

## File Structure

The submission has the following structure

├── README.md
├── Project1.pdf                            #project description
├── Checkpoints/                            #THESE WILL BE HANDED IN SEPARATELY
│   └── CNN_model.pt                        #baseline cnn model weights
│   └── model.pth                           #better model with custom architecture weights
│   └── PneumoniaResnet.pth                 #finetuned RestNet50 weights
│   └── PneumoniaResnet_random.pth          #finetuned ResnNet50 weights (with labels randomization)
└── Notebooks/
│    └── Task_1.ipynb                       #all the code for task 1
│    └── Task_2_transfer.ipynb              #training of the finetuned ResNet50 
│    └── Task_2_Randomization.ipynb         #training of the finetuned ResNet50 with randomized labels
│    └── Task_2_Gradcam.ipynb               #implementation of the Grad-CAM explainability method
│    └── Task_2_IntegratedGradients.ipynb   #implementation of the Integrated Gradients explainability method
├── requirements.txt                        #required packages to use the code