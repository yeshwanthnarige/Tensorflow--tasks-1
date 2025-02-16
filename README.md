# Tensorflow--tasks-1

TensorFlow Model Training & Analysis
This project covers essential TensorFlow operations, including tensor manipulations, loss function comparisons, optimizer performance analysis, and TensorBoard logging. The tasks were implemented step by step with explanations.

Student Information
Name: Yeshwanth Narige , ID: 700764035
University: University of Central Missouri
Email: yeshwanthnarige1313@gmail.com

Project Tasks
1. Tensor Manipulations & Reshaping
Created a random tensor of shape (4, 6).
Found its rank and shape before and after reshaping.
Reshaped it to (2, 3, 4) and transposed it to (3, 2, 4).
Applied broadcasting to add a smaller tensor (1, 4) to the larger tensor.
📌 Broadcasting Explanation:
Broadcasting allows smaller tensors to be automatically expanded to match the shape of larger tensors without explicit copying. This is useful for element-wise operations.

2. Loss Functions & Hyperparameter Tuning
Defined true values (y_true) and predicted values (y_pred).
Computed Mean Squared Error (MSE) and Categorical Cross-Entropy (CCE).
Modified predictions slightly and observed loss variations.
Plotted a bar chart comparing MSE and CCE loss values.
🔍 Key Insight:

MSE is sensitive to small changes, whereas CCE penalizes incorrect predictions more aggressively.
Loss values change significantly when predictions are modified.

3. Train a Model with Different Optimizers
Loaded the MNIST dataset (handwritten digits).
Trained two models:
Adam Optimizer
SGD Optimizer
Compared training & validation accuracy trends.
📊 Comparison:

Adam converges faster due to adaptive learning rates.
SGD takes longer but may generalize better in some cases.

4. Train a Neural Network and Log to TensorBoard
Loaded and preprocessed the MNIST dataset.
Built a simple neural network for classification.
Enabled TensorBoard logging to track training.
Launched TensorBoard to analyze:
Training vs. Validation Loss
Training vs. Validation Accuracy
📌 Stored logs in: "logs/fit/"

4.1 Questions & Answers
1. Patterns in Training & Validation Accuracy:
Overfitting occurs if validation accuracy stops improving while training accuracy increases.

2. Using TensorBoard to Detect Overfitting:
Check if validation loss starts increasing while training loss keeps decreasing.

3. Effect of Increasing Epochs:
Too many epochs can lead to overfitting.
Early stopping can prevent unnecessary training.
