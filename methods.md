Code (Android App for HAR)
•	Methods
1.	The concept leverages the built-in sensors of the phone, using them we can predict the movement / activity of a user.
2.	Permission handler is used to ask permission from the user to access the sensors.
3.	Activity Recognition package is used to tap in sensors for movement detection
4.	initState() is created so that the widget can be configured later
5.	_init() is used to ask for permission and if the permission is allowed it starts tracking using _trackingStarted()
6.	_trackingStarted() uses activityStream class from Activity recognition package to listen on Movement a.k.a Data
7.	Now activityData() has arguments of Data and adds it to the list of _events.
8.	This _events is used and a list builder is made to show the status of activity type, confidence level and timestamp using ListTile (Widget).
 


1.	To Download the files for the App, go to: - https://drive.google.com/drive/folders/1dz7zBkJviUxgHTWGfUcb2KEyTu-CoiiC?usp=sharing

Code (TensorFlow for HAR with LSTM) 
•	Methods
1.	Importing various package and also importing data from google drive
2.	We used LSTM Neural Network which uses TensorFlow for Human Activity Recognition and the model is trained and tested giving accuracy and loss between both.
3.	LSTMs are used to classify, train and process the data based on time series data.
4.	Our model expects a fixed-length sequences as training data, so we generate sequence which contained a lot of training data.
5.	We split the data into training and testing sets.
6.	We used L2 Regularization to reduce the chance of model overfitting
7.	We Trained our data up to 50 epochs and stored the accuracy and loss of data
8.	Now we plot the Training and testing data with accuracy and loss of each.
9.	We make a confusion matrix using heatmap which tells which activity is mostly used and which favours the most, true or predicted.
