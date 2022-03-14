# Full Parking Project
Project code a Parking Lot Vehicle Detection and Tracking on Google Coral EdgeTPU. 
Project built to run on multiple EdgeTPU Iot Devices mounted on multiple cameras in a parking lot, each streaming data to centralized server which parses data for vehicular parking data management. 

Each submodule does as follows: 
- Parking Model Making contains the code to train and compile the Tensorflow Lite models to be run on Google Coral EdgeTPU.
- Parking Heroku contains code to set up a flask-socketio, websocket server deployed on Heroku
- Parking TPU Client contains code to make inferences on the TPU with tflite models and stream data to the Heroku hosted server
