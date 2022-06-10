# Plagiarism Project, Machine Learning Deployment

This repository contains code and associated files for deploying a plagiarism detector using AWS SageMaker.

## Project Overview

This project is about building a plagiarism detector that examines a text file and performs binary classification; labeling that file as either *plagiarized* or *not*, depending on how similar that text file is to a provided source text. Detecting plagiarism is an active area of research; the task is non-trivial and the differences between paraphrased answers and original work are often not so obvious.

This project will be broken down into three main notebooks:

**Notebook 1: Data Exploration**
* Loading in the corpus of plagiarism text data.
* Exploring the existing data features and the data distribution.

**Notebook 2: Feature Engineering**

* Cleaning and pre-processing the text data.
* Defineing features for comparing the similarity of an answer text and a source text, and extract similarity features.
* Selecting "good" features, by analyzing the correlations between different features.
* Createing train/test `.csv` files that hold the relevant features and class labels for train/test data points.

**Notebook 3: Train and Deploy The Model in SageMaker**

* Uploading train/test feature data to S3.
* Defineing a binary classification model and a training script.
* Training the model and deploy it using SageMaker.
* Evaluate the deployed classifier.

---
