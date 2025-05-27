📊 LSTM Data Reshaping Function
Overview
This module provides a function to reshape datasets into the appropriate 3D format required for training Long Short-Term Memory (LSTM) models. LSTMs expect input in the shape of [samples, time steps, features]. This function simplifies the preprocessing step and ensures compatibility with Keras/TensorFlow LSTM layers.

🔧 Features
Reshapes 2D data into 3D format.

Supports flexible time step configuration.

Ready for use in time-series forecasting and sequence modeling.

📁 Function Description
reshape_for_lstm(X, time_steps)
Parameter	Type	Description
X	ndarray	Input 2D array of shape [samples, features]
time_steps	int	Number of time steps for LSTM input

🔄 Returns: 3D NumPy array of shape [samples, time_steps, features]

✅ Example Usage
python
Copy
Edit
import numpy as np
from lstm_utils import reshape_for_lstm

# Sample input data
X = np.array([[1, 2], [3, 4], [5, 6]])
time_steps = 1

# Reshape for LSTM
X_reshaped = reshape_for_lstm(X, time_steps)
print(X_reshaped.shape)  # Output: (3, 1, 2)
📌 Requirements
Python 3.x

NumPy

(Optional) TensorFlow/Keras for further LSTM model development

📃 License
This project is licensed under the MIT License. Feel free to use and modify it as needed.

🙋‍♂️ Author
Md Mahfuzur Rahman Siam
Software Tester & Programmer | Research & Community Support
📫 Email: ksiam3409@gmail.com or LinkedIn: https://www.linkedin.com/in/md-mahfuzur-rahman-siam/
