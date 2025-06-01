Sudent name: Aditya Kumar Dupakuntla
Sudent id: 700773563


1. Tensor Manipulations & Reshaping (TensorFlow)
This task demonstrates basic tensor operations using TensorFlow:

-> Created a random tensor of shape (4, 6).

-> Computed its rank and shape.

-> Reshaped it to (2, 3, 4) and transposed to (3, 2, 4).

-> Used broadcasting to add a smaller tensor of shape (1, 4) to the transposed tensor.

-> Broadcasting automatically expands tensors to compatible shapes for element-wise operations.

This exercise showcases key tensor manipulation techniques like reshaping, transposing, and broadcasting in TensorFlow.

2. Loss Functions & Hyperparameter Tuning (TensorFlow)
This task compares how different loss functions respond to changes in model predictions:

-> Defined true labels and two sets of predicted outputs (original and slightly modified).

-> Computed:

Mean Squared Error (MSE)

Categorical Cross-Entropy (CCE)

-> Observed how loss values change with prediction tweaks.

-> Visualized the comparison using a bar chart.

This helps in understanding the sensitivity of different loss functions and their behavior during model training.

3. Train a Neural Network and Log to TensorBoard (MNIST)
This task demonstrates training a neural network on the MNIST dataset with TensorBoard logging:

-> Loaded and preprocessed the MNIST dataset (normalized and one-hot encoded).

-> Built and trained a simple neural network for digit classification.

-> Enabled TensorBoard logging via tf.keras.callbacks.TensorBoard.

-> Trained for 5 epochs and saved logs to logs/fit/.

-> Visualized training vs. validation accuracy and loss using TensorBoard

4)  1. What patterns do you observe in the training and validation accuracy curves?
Answer:
•	Training accuracy typically increases steadily.
•	Validation accuracy should follow closely if the model generalizes well.
•	A large gap (training ↑, validation ↓ or flat) indicates overfitting.

    2. How can you use TensorBoard to detect overfitting?
Answer:
•	Check loss curves:
o	If training loss keeps decreasing but validation loss increases → overfitting.
o	Training accuracy increases while validation accuracy stalls or drops.
•	TensorBoard makes it easy to visually detect this divergence.

    3. What happens when you increase the number of epochs?
Answer:
•	Initially:
o	Both training and validation accuracy improve.
o	Training accuracy continues to improve.
o	Validation accuracy plateaus or decreases → overfitting risk increases.
•	Solution: Use techniques like EarlyStopping or regularization.
