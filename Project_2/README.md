 
# PROJECT 2

## Group components:
Sophia Houhamdi, Eva Sarlin, Lorenzo Tarricone


## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [File Structure](#file-structure)

## Introduction

Project 2 focuses on working with time series from ECG datasets for classification of the status of the patient. We analyzed the pubblicly available [PTB Diagnostic ECG Database](https://physionet.org/content/ptbdb/1.0.0/) and [MIT-BIH Arrhythmia Database](https://physionet.org/physiobank/database/mitdb/) It consists of three parts: 
1. The first part consists in producing many different models for the classsification of the PTB dataset.These include classic models (logistic regression, Random Forests, Support Vector Machine) and more recent Deep Learning architectures (CNN, LSTM and Tranformer encoder)
2. The second part deals with creating good embeddings by exploring differnet techniques of representaion and tranfer learning.
3. The third part involves summarizing findings, answering general questions about the methods used, and exploring pros and cons of all the mdoel implemented. 

## Features

In our implementation of the constrastive learning InfoNCE was adapted form [here](https://github.com/jefflai108/Contrastive-Predictive-Coding-PyTorch.git))

## Installation

A `requirement.txt` file is provided containig all the packages we used for this project. In order to install them you can simply run. To ensure they are all installed in your current environment please run

`pip install -r requirements.txt`

## Usage

Once you have all the needed packages in your envuroment as described above, you can simply open the notebook correponding to the section you are interested in and run the code smoothly.

## File Structure

The submission has the following structure

├── README.md                               #this file
├── Project2.pdf                            #project description
├── Report.pdf                              #report for teh question in the project descritpion
└── Notebooks/
│    └── Part_1_Q1&2_classicML.ipynb        #implementation of Classic ML algorithms
│    └── Part_1_Q3_LSTM.ipynb               #implementation of LSTM architecture
│    └── Part_1_Q4_CNN_Complex.ipynb        #implementation of the big CNN architecture (5 convolutional blocks)
│    └── Part_1_Q4_CNN_Simple.ipynb         #implementation of the big CNN architecture (1 convolutional blocks)
│    └── Part_1_Q5_Transformer.ipynb        #implementation of the transformer architecture + attention maps
│    └── Part_2_CPC.ipynb                   #implementation of the constastive loss-based-architecture
│    └── Part_2_Simple_CNN.ipynb            #implementation of the simple CNN architecture used for contrastive loss embeddings
├── requirements.txt                        #required packages to use the code