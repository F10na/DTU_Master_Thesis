# DTU_Master_Thesis
Predicting task from gaze data using a neural network trained on sequences of detected eye movements
15 July 2022
Isabella A. Moreno Schøning

This project is the source code for the above-mentioned Master thesis. The thesis has been prepared over five months at the Section for Cognitive Systems,
Department of Applied Mathematics and Computer Science, at the Technical University of Denmark, DTU, in partial fulfilment for the degree Master of Science in Engineering, MSc Eng.

The purpose of the project is determine if it is possible to predict a person's task based on their eye movements. To do so, I train a supervised neural network on sequences of detected eye movements from gaze data labelled by task. The algorithm has been tested on two eye trackers: Pupil Invisible glasses and Varjo XD. The solution is broken into two parts:

1. Detecting eye movement events in gaze data via a native EM-GMM probabilistic approach.
2. Predicting task from the outputted event sequences using a supervised neural network.

## Event_Detection
main_GMM_out: Detects fixations, smooth pursuits, saccades and blinks given positional time-series gaze data from an eye tracker. Output is a csv of concatenated event sequenes with features.

main_GMM_results: Analyzes the output csv file, including graphs.

event_sequences.csv: The resulting event sequences of all gaze datasets, combined into one csv. Each event includes features such as duration, amplitude, maximum speed. Also included are the joint probabilities of each event.

## Task_Prediction


## Explanation of Data
The data from Pupil Invisible contains personal information and is therefore not to be distributed. This data can only be accessed via a secure DTU server.
The data from the Varjo are recorded personally and are provided in the folder "Varjo Experiments". This data is not IP.
