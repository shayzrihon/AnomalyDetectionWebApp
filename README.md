# AnomalyDetectionWebApp
This project was coded in C++, JavaScript and HTML.  In the project one can run an anomaly detection server, using Node.js.
To do so download the program. 
Then in the directory "Model" run the command "node-gyp configure" and " node-gyp build" then from the directory "Controller" run the command npm start. 
This may require installing  packages: "npm i express" and "npm i express-fileupload".		
sudo apt install node-gyp
sudo apt install npm

The server can then be accessed through a web browser in the address localhost:8080. 
The web browser asks the user to upload two CSV files of the user's choice, one for training and one for testing the anomaly detector.
The user may choose which anomaly detection algorithm to use (regression or hybrid). 
After clicking submit, the data is communicated to the server. 
The results (the features and timepoints in which an anomaly was detected) will be displayed on the web page.

One can also run the program using one HTTP POST command, 
which contains the paths to the CSV files, and the choice of anomaly detection algorithm to be used (regression or hybrid). 
The anomalies will appear in a json object.
