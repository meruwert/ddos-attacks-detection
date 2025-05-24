Project: DDoS Detection Using Deep Learning (CICIDS2017 & CICDDoS2019)

This folder contains the core source code and scripts used for training, testing, and evaluating machine learning models for the detection of distributed denial-of-service (DDoS) attacks. The experiments are based on publicly available datasets CICIDS2017 and CICDDoS2019, and include both deep learning (DNN) and classical machine learning approaches (e.g., SVM).

File Descriptions
1. maintrain(2).ipynb

This is the primary training notebook that preprocesses the CICDDoS2019 dataset and trains a Deep Neural Network (DNN) for binary classification (attack vs. benign). It includes:

    Data loading and cleansing (NaN and infinite value removal)

    Feature normalization

    Class balancing via resampling

    DNN architecture setup with dropout layers

    Model training and validation

    Exporting the trained model

2. side training cicid2017.ipynb

This notebook contains auxiliary experiments using the CICIDS2017 dataset. It follows a similar pipeline to the main training notebook but adapts the feature space and labels to match the structure of the 2017 dataset. This is used to test generalization performance across datasets.
3. server TEST

This is a folder or file used during the server-based emulation testing phase. It may include:

    Scripts for deploying the trained model in a simulated server environment

    Network traffic emulation (normal and DDoS scenarios)

    Evaluation of the model in real-time or batch inference

Dependencies

These scripts require the following environments and packages:

    Python 3.8+

    TensorFlow 2.x

    Pandas, NumPy

    Scikit-learn

    Google Colab or Jupyter environment for .ipynb execution
