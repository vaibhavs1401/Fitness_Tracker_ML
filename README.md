# Fitness_Tracker_ML

**Barbell Exercise Classification and Repetition Counting Using Sensor Data**
This project focuses on processing, visualizing, and modeling accelerometer and gyroscope data to build a machine learning model capable of classifying barbell exercises and counting repetitions. It was developed as part of the Machine Learning for the Quantified Self course from the Master Artificial Intelligence program at Vrije Universiteit Amsterdam.

**Project Overview
Goal**
The main goal of this project is to create Python scripts to:

Process and visualize sensor data (accelerometer and gyroscope).
Engineer features that enhance classification performance.
Build a machine learning model that classifies barbell exercises and counts repetitions.
Dataset
The dataset consists of raw accelerometer and gyroscope data collected during gym workouts, where participants (5 total) performed various barbell exercises. Each dataset is labeled by exercise, participant, and intensity level (e.g., light, medium, heavy).

Sensor Used
The data was collected using the MetaMotion Sensor from Mbientlab, which provides 6-DOF motion data (3-axis accelerometer and 3-axis gyroscope).

**Project Structure**
The project is divided into several key parts:

**Data Preprocessing**

Reads multiple CSV files containing raw sensor data.
Extracts features such as participant, exercise type, and intensity from the file names.
Cleans and merges the data into a unified format for analysis.
**Data Visualization**

Plots time series data of accelerometer and gyroscope measurements.
Visualizes comparisons between different exercises, participants, and intensity levels.
**Outlier Detection**

Implements outlier detection using methods like Interquartile Range (IQR), Chauvenet’s Criterion, and Local Outlier Factor (LOF).
Cleans the data by replacing outliers before further processing.
**Feature Engineering**

Applies techniques such as low-pass filtering and Principal Component Analysis (PCA) to extract key features from the sensor data.
Temporal and frequency abstraction for more meaningful features.
Clustering to identify similar motion patterns across exercises.
**Predictive Modeling**

Builds machine learning models such as Naive Bayes, SVM, Random Forest, and Neural Networks to classify barbell exercises.
Conducts hyperparameter tuning using grid search to improve model accuracy.
**Repetition Counting**

Custom algorithm to count repetitions of each exercise based on the sensor data peaks.
Visualizes the filtered data with identified peaks for repetitions.
Dependencies
The project uses the following dependencies, which can be installed using the provided environment.yml file:

**Python 3.8+
Pandas
NumPy
Matplotlib
Scikit-learn
SciPy
Seaborn
MetaMotion SDK (optional for sensor data collection)
Jupyter Notebook (optional for development)**
