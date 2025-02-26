Task 1: Basic Digit Classification

Dataset: 28x28 grayscale digit images (e.g., Kaggle’s Digit Recognizer)

Preprocessing:

Flatten images into 784-dimensional vectors

One-hot encode labels (0-9)

Model:

Sequential model with 784 input neurons and 10 output neurons (Softmax activation)

No hidden layers

Training:

RMSprop optimizer

Categorical crossentropy loss

Trained for 10 epochs

Observations:

Baseline performance established

Loss and accuracy curves show initial trends in model performance

Task 2: Batch Size Tuning

Experiment:

Trained using batch sizes of 1000 and 2000

Compared loss and accuracy curves

Observations:

Larger batch size (2000) led to more stable training

Fewer updates per epoch resulted in smoother convergence

Task 3: Optimizer Adjustment

Experiment:

Used AdaDelta (learning rate 0.01) and trained for 20 epochs

Switched to Adam (learning rate 0.05) and trained for 20 epochs

Observations:

Adam showed better convergence and improved performance compared to AdaDelta

Faster learning and lower final loss

Task 4: Hidden Layer Addition

Model Modification:

Added a hidden layer with 50 units and ReLU activation

Output layer remained Softmax with 10 neurons

Training:

Used Adam optimizer with a learning rate of 0.05

Trained for 20 epochs

Observations:

Increased model capacity improved accuracy

Potential overfitting noticed in loss curves

Task 5: Dropout Application

Model Modification:

Added a Dropout layer (0.2) after the hidden layer

Training:

Used Adam optimizer (learning rate 0.05)

Trained for 20 epochs

Observations:

Dropout reduced overfitting by narrowing the train-test accuracy gap

More stable generalization observed

Task X (Bonus): Regression Tuning

Dataset: Regression dataset (e.g., California Housing Prices)

Model:

Input layer matching feature count

Hidden layer with 20 ReLU units

Output layer with a single neuron

Training:

Used RMSprop optimizer (learning rate 0.01)

Mean Squared Error (MSE) as loss function

Trained for 30 epochs

Observations:

Dropout (0.1) improved stability

Reduced overfitting compared to no dropout model
