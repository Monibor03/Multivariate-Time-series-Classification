This work focuses on multivariate time series classification using deep learning at Jefferson Lab, Virginia.

The process begins with extracting raw data from the lab’s data server. From each superconducting cavity, we select 4 specific signals out of 17 available. Signals from all 8 cavities within a cryomodule are then combined for analysis. The data undergoes several preprocessing steps, including downsampling, train-validation-test splitting, and channel-wise normalization.

Following preprocessing, we train a deep learning model based on a hybrid LSTM-CNN architecture. The model is trained on the training set and validated using the validation set, with training stopping automatically when the validation loss reaches its minimum. After training, we evaluate the model on the test set to assess its generalization performance.

Finally, the trained model is deployed in the Jefferson Lab control room to perform real-time fault classification and identify faulty cavities, supporting operational stability and diagnostics.
