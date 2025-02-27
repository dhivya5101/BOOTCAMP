

## Manual Backpropagation

#### Task 1: Manual Backpropagation
- **Understanding a simple regression problem**
  - Used a dataset with 4 features (e.g., height, weight, age, smoking) and a target variable (premium).
- **Defined a mini neural network**
  - Input layer: 4 features
  - Hidden layer: 2 units
  - Output layer: 1 unit (no activation function)
  - Initialized weights manually.
- **Forward Pass Computation**
  - Calculated hidden layer activations and final output.
- **Loss Calculation**
  - Used Mean Squared Error (MSE) formula to compute the error.
- **Backpropagation via Chain Rule**
  - Derived weight gradients using differentiation.
  - Updated one weight manually (e.g., W1).
- **Key Takeaway:**
  - Demonstrated how weight updates follow the chain rule in backpropagation.

---

## Feedforward Linear Limitation

#### Task 2: Feedforward Network Performance
- **Tested Linear Regression with a Feedforward Network**
  - Used the same dataset but introduced a computed nonlinear feature (BMI = weight/height²).
- **Built a Feedforward Network**
  - 4 input features → 2 hidden units → 1 output.
- **Trained with and without BMI Feature**
  - Used RMSprop optimizer and MSE loss.
- **Plotted Loss Curve**
  - Compared performance with and without BMI input.
- **Key Takeaway:**
  - Feedforward networks struggle to capture nonlinearity unless explicitly included in input features.

---

## Basic CNN Convolution

#### Task 3: Convolution Operation
- **Sourced an image dataset (28x28 grayscale digits).**
- **Defined a Single 3x3 Filter**
  - Example: Diagonal edge detection filter.
- **Applied Convolution using TensorFlow (tf.nn.conv2d).**
- **Visualized the Feature Map (26x26 output).**
- **Key Takeaway:**
  - Learned how filters extract features from images, e.g., detecting edges.

---

## Multi-Filter CNN

#### Task 4: Multiple Filters in CNN
- **Built a CNN Model with 3 Filters (3x3 each).**
- **Flattened Image to 784 Inputs and Classified into 10 Categories.**
- **Compiled Model with Adam Optimizer and Categorical Crossentropy.**
- **Trained for 10 Epochs and Extracted Feature Maps.**
- **Key Takeaway:**
  - Multiple filters help capture diverse image features, improving classification accuracy.

---

## CNN Weight Updates

#### Task 5: Monitoring CNN Learning
- **Used the CNN Model from Task 4.**
- **Trained for 20 Epochs While Monitoring Loss and Accuracy.**
- **Extracted and Visualized Weight Changes Before and After Training.**
- **Plotted Loss and Accuracy Curves.**
- **Key Takeaway:**
  - Observed weight evolution and confirmed backpropagation’s effect on learning.

---

## Bonus: Comparing Feedforward & CNN

#### Task X: Image Regression with Feedforward vs. CNN
- **Sourced an Image Dataset for Regression (Predicting Brightness).**
- **Built and Trained Two Models:**
  - Feedforward Network: 784 Inputs → 2 Hidden Units → 1 Output.
  - CNN: 1 Filter (3x3) → Flatten → 1 Output.
- **Trained Both for 10 Epochs Using MSE Loss.**
- **Compared Loss Curves and Discussed Feature Extraction Differences.**
- **Key Takeaway:**
  - CNNs extract spatial features, while feedforward networks rely on explicit feature engineering.

---
