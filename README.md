# Gaussian Mixture Model for Anomaly Detection

This repository contains the implementation of a Gaussian Mixture Model (GMM) for anomaly detection. The project involves training and evaluating multiple models to identify the best-performing one based on various metrics.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Models](#models)
- [Evaluation Metrics](#evaluation-metrics)
- [Results](#results)
- [Usage](#usage)
- [Installation](#installation)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project implements a Gaussian Mixture Model (GMM) for detecting anomalies in a dataset. Several models with different parameters were trained and evaluated to determine the best one based on metrics like AUC, F1 Score, Precision, and Recall.

## Dataset

The dataset used for this project includes multiple features relevant to the detection of anomalies. The data is split into training, validation, and test sets. The training and validation sets are used to train and optimize the models, while the test set is used for final evaluation.

## Models

The following models were trained and evaluated:

1. **Model-1**: 3 features, 3 components, 1 Gaussian
2. **Model-2**: 2 features, 3 components, 1 Gaussian
3. **Model-3**: 2 features, 1 component, 1 Gaussian
4. **Model-4**: 2 features, 1 component, 1 Gaussian (poor performance)
5. **Model-5**: 2 features, 1 component, 1 Gaussian
6. **Model-6**: 2 features, 3 components, 1 Gaussian
7. **Model-7**: 10 features, 1 component, 1 Gaussian (best performance)
8. **Model-8**: 10 features, 1 component, 1 Gaussian (poor performance)
9. **Model-9**: 10 features, 5 components, 1 Gaussian (poor performance)
10. **Model-10**: 2 features, 1 & 3 components, 2 Gaussians (not evaluated)

## Evaluation Metrics

The models were evaluated using the following metrics:

- **AUC (Area Under the Curve)**: Measures the ability of the model to distinguish between classes.
- **F1 Score**: Harmonic mean of precision and recall.
- **Precision**: Ratio of correctly predicted positive observations to the total predicted positives.
- **Recall**: Ratio of correctly predicted positive observations to the all observations in actual class.

## Results

The best model, Model-7, was evaluated on the test set with the following results:

- **AUC**: 0.9781
- **F1 Score**: 0.7154
- **Precision**: 0.8000
- **Recall**: 0.6471

## Usage

To use this project, follow these steps:

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/gaussian-mixture-model-anomaly-detection.git
    cd gaussian-mixture-model-anomaly-detection
    ```

2. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

3. Run the model training and evaluation script:
    ```sh
    python train_and_evaluate.py
    ```

4. The results will be printed in the console and saved to a file named `results.txt`.

## Installation

Ensure you have Python 3.6 or higher installed. Install the dependencies using the following command:

```sh
pip install -r requirements.txt
