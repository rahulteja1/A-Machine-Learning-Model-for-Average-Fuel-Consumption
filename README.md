# A Machine Learning Model for Average Fuel Consumption

## Overview
This project aims to predict the average fuel consumption of heavy vehicles using a Machine Learning model, specifically an Artificial Neural Network (ANN). The dataset comprises various features extracted from the vehicle's travel data, which are used to train and test the ANN model. The end goal is to optimize fuel consumption across a fleet of vehicles by predicting fuel usage based on these features.

## Dataset
The dataset used in this project includes the following features:

1. **num_stops**: Number of times the vehicle stops.
2. **time_stopped**: Total time the vehicle is stopped.
3. **average_moving_speed**: Average speed of the vehicle when it is in motion.
4. **characteristic_acceleration**: Rate of acceleration of the vehicle.
5. **aerodynamic_speed_squared**: A measure of aerodynamic drag.
6. **change_in_kinetic_energy**: Change in the kinetic energy of the vehicle.
7. **change_in_potential_energy**: Change in the potential energy of the vehicle.
8. **class**: Represents fuel consumption for the vehicle.

The dataset is divided into training and testing sets in an 80-20 ratio. The training set is used to build the ANN model, while the testing set is used to evaluate the model's performance.

## Project Modules

### 1. Upload Heavy Vehicles Fuel Dataset
This module allows you to upload the dataset containing the vehicle travel data. The dataset is a CSV file where each row represents a vehicle's data over a 100 km travel distance.

### 2. Read Dataset & Generate Model
This module parses the uploaded dataset and generates the training and testing datasets. The ANN model is built using the training data, while the testing data is reserved for model evaluation.

### 3. Run ANN Algorithm
This module creates the ANN model, feeds it the training data, and trains the model to predict fuel consumption. The training process includes splitting the dataset into training and testing sets, feeding the data into the ANN, and adjusting the model parameters.

### 4. Predict Average Fuel Consumption
Once the model is trained, this module allows you to upload new test data. The ANN model is then applied to this test data to predict the average fuel consumption.

### 5. Fuel Consumption Graph
This module generates a graph that plots the predicted fuel consumption for each test record. The x-axis represents the vehicle ID (or test record number), and the y-axis represents the predicted fuel consumption per 100 km.

## ANN Working Procedure
The ANN model is developed using a dataset collected from a single truck with a mass of approximately 8,700 kg. The truck was exposed to various driving conditions, including both urban and highway traffic, in the Indianapolis area. The dataset was collected using the SAE J1939 standard, which is commonly used for serial control and communications in heavy-duty vehicle networks.

The ANN model consists of multiple layers of neurons, where each neuron performs a mathematical operation on the input data. The output from one layer is passed as input to the next layer until the final output is obtained, representing the predicted fuel consumption.

## Running the Project

1. **Start the application**: Run the `run.bat` file to start the application.
2. **Upload Dataset**: Click on the "Upload Heavy Vehicles Fuel Dataset" button to upload the training dataset (`Fuel_Dataset.txt`).
3. **Generate Model**: Click on "Read Dataset & Generate Model" to parse the dataset and generate training and testing datasets.
4. **Run ANN Algorithm**: Click on "Run ANN Algorithm" to train the ANN model using the training data.
5. **Predict Fuel Consumption**: Click on "Predict Average Fuel Consumption" to upload new test data and predict fuel consumption.
6. **View Results**: The results, including prediction accuracy and fuel consumption graph, will be displayed.

## Conclusion
This project demonstrates how to use an ANN model to predict the average fuel consumption of heavy vehicles. By optimizing fuel consumption, the model can help in reducing operational costs and improving efficiency across a fleet of vehicles.

## Additional Information
- **Training Accuracy**: The model achieved an accuracy of up to 86% during training.
- **Testing**: The fuel consumption prediction for the test data is visualized through a graph, helping to analyze the model's performance across different test cases.

## Notes
- The entire dataset and test data are available inside the `dataset` folder.
- The ANN model can be further fine-tuned by experimenting with different hyperparameters and architectures to improve prediction accuracy.
