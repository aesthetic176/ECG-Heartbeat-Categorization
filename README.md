# ECG-Heartbeat-Categorization

### Dataset
Dataset Link : https://www.kaggle.com/datasets/shayanfazeli/heartbeat
### Code Explanation

The above code is developed for binary classification, aimed at distinguishing between healthy (normal) and anomalous (abnormal) heartbeats using ECG signal data. This task is crucial in medical diagnostics, particularly in the detection and monitoring of heart conditions.

The process begins with loading four separate datasets. Two of these datasets, labeled as 'ptbdb_normal' and 'ptbdb_abnormal', contain ECG signals representing normal and abnormal heartbeats, respectively. The other two datasets, 'mitbih_train' and 'mitbih_test', likely consist of a mixed collection of both normal and abnormal heartbeats.

After loading the datasets, the code combines them into a single dataset, creating a more comprehensive collection for analysis. It then separates the ECG signals (features) and their corresponding labels (normal or abnormal) into 'X' and 'y' variables.

An essential step in the preparation of the data involves handling missing or invalid values, known as NaNs (Not a Number), and ensuring all labels are correctly formatted as 0 (normal) or 1 (abnormal) for binary classification. This preparation is crucial for the accuracy and reliability of the classification model.

The code then standardizes the ECG signals, a process that normalizes the data to ensure uniformity and comparability. This step is vital for effective model training and prediction accuracy.

The next phase involves reshaping the standardized data to fit a Convolutional Neural Network (CNN) model. CNNs are highly effective in pattern recognition tasks, making them suitable for analyzing ECG signals. The data is divided into training and testing sets, allowing the model to learn from one set and validate its learning on the other.

The model architecture includes Convolutional, MaxPooling, Flatten, Dropout, and Dense layers, structured to extract significant features from the ECG signals and classify them accurately. The model is compiled with an Adam optimizer and a lower learning rate to enhance training stability.

After training the model with the specified number of epochs and batch size, its performance is evaluated using the testing data set. The accuracy metric provides insight into how well the model differentiates between normal and abnormal heartbeats.

In conclusion, this code represents a comprehensive approach to using machine learning, particularly CNNs, for the critical task of identifying heart conditions through ECG signal analysis.
