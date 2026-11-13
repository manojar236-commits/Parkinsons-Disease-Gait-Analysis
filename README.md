# Early Detection and Severity Classification of Parkinson's Disease Using Gait Analysis and Deep Learning

## Project Overview

Parkinson's disease is a progressive neurological disorder that affects movement, balance, and coordination. Gait analysis can help identify movement-related changes associated with Parkinson's disease.

This project focuses on the early detection and severity classification of Parkinson's disease using gait data and deep learning techniques.

The system analyzes gait measurements, processes the data, and uses a deep learning model to estimate Parkinson's disease probability and classify disease severity.

## Objectives

* Analyze gait data from healthy individuals and individuals with Parkinson's disease.
* Preprocess and prepare gait measurements for model training.
* Develop a deep learning model for gait pattern analysis.
* Estimate the probability of Parkinson's disease.
* Classify severity into Healthy, Mild, Moderate, and Severe categories.
* Evaluate model performance using test data.

## Dataset

**Dataset:** Gait in Neurodegenerative Disease Database

**Source:** PhysioNet

The dataset contains gait measurements from healthy control subjects and subjects with neurological disorders, including Parkinson's disease.

Dataset link: https://physionet.org/content/gaitndd/1.0.0/

The project uses gait data files to extract numerical measurements for analysis.

## Technologies Used

* Python
* Google Colab
* TensorFlow / Keras
* NumPy
* Pandas
* Scikit-learn
* Matplotlib
* Deep Learning
* Bidirectional LSTM (BiLSTM)

## Project Workflow

1. Dataset collection
2. Data loading
3. Data preprocessing
4. Gait feature preparation
5. Feature scaling
6. Deep learning model development
7. Model training and testing
8. Parkinson's disease probability estimation
9. Severity classification
10. Performance evaluation

## Model Architecture

The project uses a Bidirectional Long Short-Term Memory (BiLSTM) based deep learning architecture.

The model includes:

* Bidirectional LSTM layers
* Dropout layers
* Dense layers with ReLU activation
* Softmax output layer

The model is trained using the Adam optimizer and Sparse Categorical Crossentropy loss function.

## Classification Categories

The project uses four output categories:

| Class | Category |
| ----- | -------- |
| 0     | Healthy  |
| 1     | Mild     |
| 2     | Moderate |
| 3     | Severe   |

The model's Parkinson's probability estimate is derived from its predicted class probabilities.

**Note:** Severity labels depend on the labeling method implemented in the project. They should not be interpreted as clinically validated severity assessments.

## Model Evaluation

The model is evaluated using a training and testing approach with an 80:20 split.

* 80% of the data is used for training.
* 20% of the data is reserved for testing.
* A confusion matrix is used to evaluate severity classification on the test data.

Actual performance metrics and graphs should be added after final model evaluation.

## Repository Contents

* `Parkinson_Gait_Analysis.ipynb` – Python implementation of the project.
* `Project_Report.pdf` – Complete project documentation.

## Future Enhancements

* Improve severity classification using clinically validated severity labels.
* Collect gait data using camera-based gait analysis.
* Explore additional deep learning architectures.
* Improve model generalization using subject-wise evaluation.
* Develop a user-friendly interface for predictions.

## Disclaimer

This project is an academic research prototype and is not intended to replace professional medical diagnosis.

## Author

Developed as an academic major project in Artificial Intelligence and Machine Learning.
