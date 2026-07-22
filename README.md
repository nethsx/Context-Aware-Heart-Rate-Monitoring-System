# Context-Aware-Heart-Rate-Monitoring-System
Machine learning-based heart rate monitoring system developed in MATLAB for activity classification and abnormality detection.

# Context-Aware Heart Rate Monitoring System

A MATLAB-based machine learning project that classifies heart rate data into **Rest** and **Physical Activity** using a Support Vector Machine (SVM). Based on the predicted activity state, the system detects **Bradycardia** and **Tachycardia**, reducing false alerts associated with fixed heart rate thresholds.

## Repository Contents

### `heartbeat.m`

* Loads the trained SVM model (`svm_model.mat`).
* Classifies heart rate data into **Rest** or **Physical Activity**.
* Detects **Bradycardia** and **Tachycardia** based on the predicted activity state.
* Performs comparative analysis between different heart rate datasets and cardiac conditions.
* Generates waveform visualizations and comparison plots.
* Displays prediction and monitoring results.

### `svm_model.m`

* Loads the Kaggle and synthesized datasets.
* Preprocesses the datasets for machine learning.
* Trains the Support Vector Machine (SVM) classifier.
* Compares the performance of multiple machine learning models.
* Evaluates the classifier using accuracy, confusion matrices, and performance metrics.
* Saves the trained model as `svm_model.mat` for use in `heartbeat.m`.

## Datasets

The project uses two categories of datasets:

* **`kaggle_datasets/`** – Original heart rate datasets obtained from Kaggle.
* **`synthesized_datasets/`** – Custom-generated datasets developed to simulate additional cardiac conditions and activity states for training and evaluation.

> **Important:** Keep both `kaggle_datasets` and `synthesized_datasets` in the same project directory as `heartbeat.m`, `svm_model.m`, and `svm_model.mat`. The MATLAB scripts are configured to load the datasets from these folders.

## Requirements

* MATLAB
* Statistics and Machine Learning Toolbox

## Running the Project

1. Clone or download this repository.
2. Ensure the following are located in the same project directory:

   * `heartbeat.m`
   * `svm_model.m`
   * `svm_model.mat`
   * `kaggle_datasets`
   * `synthesized_datasets`
3. Run `svm_model.m` to train and evaluate the SVM classifier.
4. Run `heartbeat.m` to perform heart rate classification, dataset comparison, waveform visualization, and cardiac condition detection.

## Future Scope

* Integration with real-time ECG/PPG sensors.
* Deployment on wearable devices.
* Real-time continuous heart rate monitoring.
* Expansion to additional cardiac abnormality detection.
