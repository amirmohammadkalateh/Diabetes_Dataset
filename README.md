# Diabetes_Dataset

# Diabetes Prediction Model

This project implements an Artificial Neural Network (ANN) using TensorFlow's Functional API to predict diabetes based on various health metrics.

## Dataset

The model uses the Pima Indians Diabetes Database that includes the following features:
- Pregnancies
- Glucose
- Blood Pressure
- Skin Thickness
- Insulin
- BMI
- Diabetes Pedigree Function
- Age
- Outcome (Target variable: 0 = No Diabetes, 1 = Diabetes)

## Model Architecture

The neural network consists of:
- Input layer (8 features)
- Dense layer (16 neurons, ReLU activation)
- Dropout layer (0.3 rate)
- Dense layer (8 neurons, ReLU activation) 
- Dropout layer (0.2 rate)
- Output layer (1 neuron, Sigmoid activation)

## Features

- Data preprocessing using StandardScaler
- Piecewise learning rate schedule
- Dropout layers for regularization
- Binary cross-entropy loss function
- Adam optimizer

## Requirements

- Python 3.11
- TensorFlow 2.14.0
- NumPy 2.2.4
- Pandas 2.2.3
- Scikit-learn 1.6.1

## Usage

Run the model using the Replit run button or execute:

```bash
python main.py
```

The model will:
1. Load and preprocess the data
2. Train using the specified architecture
3. Display the test accuracy

## Learning Rate Schedule

The model implements a piecewise learning rate schedule with:
- Initial learning rate: 0.001
- Decay steps: 1000
- Decay rate: 0.9
