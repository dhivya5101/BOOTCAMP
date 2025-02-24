
### Task 1: Housing Price Regression
- **Dataset Handling**: Loaded a housing dataset, extracted features (`X`) and target (`y`), and performed train-test split.
- **Model Architecture**: Built a simple neural network with no hidden layers, just an input layer and an output neuron.
- **Compilation & Training**: Used RMSprop optimizer and Mean Squared Error (MSE) loss function.
- **Evaluation**: Observed how the model learns over 20 epochs by plotting training and validation loss.
- **Insight**: A single-layer model may be too simple to capture complex patterns in housing prices.

### Task 2: Digit Recognition
- **Data Preprocessing**: Flattened 28x28 grayscale images into 784 inputs and applied one-hot encoding for labels.
- **Model Design**: Created a simple feedforward neural network with Softmax activation for multi-class classification.
- **Training & Evaluation**: Trained for 10 epochs using categorical crossentropy loss and RMSprop optimizer.
- **Prediction Visualization**: Evaluated accuracy and visualized sample digit predictions.
- **Insight**: Even a simple neural network can perform well on digit classification tasks.

### Task 3: Batch Size Adjustment
- **Batch Size Experimentation**: Trained the regression model with batch sizes of 16, 32, and 64.
- **Observations**:
  - Smaller batch sizes resulted in more updates per epoch but higher variability.
  - Larger batch sizes led to smoother but potentially slower convergence.
  - Mini-batch count calculation aligned with expected values based on dataset size.

### Task 4: Optimizer Comparison
- **Comparing RMSprop & Adam**: Trained the digit recognition model with both optimizers.
- **Loss & Accuracy Plots**:
  - RMSprop showed steady learning but required careful tuning.
  - Adam converged faster and provided higher accuracy.
- **Conclusion**: Adam generally performs better for classification due to adaptive learning rate adjustments.

### Task 5: Hidden Layer Tuning
- **Adding Hidden Layers**: Introduced a 2-unit ReLU hidden layer to the regression model.
- **Impact on Training**: Observed lower training loss compared to the single-layer model.
- **Further Tuning**: Increased hidden units to 4, which improved performance slightly.
- **Key Takeaway**: Properly tuned hidden layers help neural networks learn more complex relationships in data.

### Bonus Task X: Regression vs. Classification
- **Combining Both Models**: Implemented separate models for regression and classification.
- **Comparing Processes**:
  - Regression used MSE loss and RMSprop optimizer.
  - Classification used categorical crossentropy loss and Adam optimizer.
- **Insights**:
  - Classification tasks often benefit from Adam due to fast convergence.
  - Regression tasks need careful tuning of hidden layers and batch sizes.

