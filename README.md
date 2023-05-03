# Overview:
This project aims to recognize hand gestures using the MediaPipe library and the Random Forest Classifier machine learning algorithm. The project consists of four Python scripts that collect training data, preprocess the data, train the model and use the model to recognize hand gestures in real-time.

# Requirements:

Python 3.6 or higher
OpenCV library
MediaPipe library
Scikit-learn library
Matplotlib library
Installation:

# Clone the repository from GitHub.
Install the required libraries by running the following command:
pip install -r requirements.txt

#Usage:
Collect training data by running the "collect_data.py" script. This will record video input from the default camera and save it to the "data" folder. The script will prompt the user to press the "Q" key to start recording and save 100 frames for each gesture. The default number of classes is 3, but this can be changed by modifying the "number_of_classes" variable.
Preprocess the data by running the "preprocess_data.py" script. This will extract the hand landmarks using the MediaPipe library and save the preprocessed data to a pickle file named "data.pickle" in the project directory.
Train the model by running the "train_model.py" script. This will split the preprocessed data into training and testing sets, train a Random Forest Classifier model, and save the model to a pickle file named "model.p" in the project directory.
Recognize hand gestures in real-time by running the "recognize_gestures.py" script. This will open the default camera and display the video feed with the recognized gesture displayed on the screen. The script will use the trained model to predict the gesture in real-time.
Contributing:
Contributions to this project are welcome. If you find any issues or have any suggestions, please open an issue or pull request on GitHub.

# License:
This project is licensed under the MIT License. See the LICENSE file for more details.
