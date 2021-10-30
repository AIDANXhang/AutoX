# Autopilot
We implemented three different Regression models, they predict a series of Steering Wheel Angles for a series of video frames.

                       **This Project was under the guidance of Dr. Shiv Ram Dubey**

# Problem Statement: 
Given a series of video frames, we want to predict a series of Steering Wheel Angles to achieve automatic steering in autopilot mode. We wanted to build a model to
make the solution simple, effective and efficient.

# Dataset collection and Dataset used:
https://github.com/SullyChen/driving-datasets
Format :- filename.jpg, angle, year-mm-dd hh:min:sec:millisec
This dataset consists of approximately 63,000 images, consisting of 3.1GB. Data was recorded around Rancho Palos Verdes and San Pedro California.

    Link to a detailed report on this project: https://drive.google.com/file/d/1ieO5-zvVFa503gHy6beJW3eWzq76YD1s/view?usp=sharing

# Observation:
From the 3 models we designed, model1 converged fast though the initialisation was truncated normal, but inception model that was pre trained on imagenet had good initialisation but at a point it was stuck, tried changing learning rate as well as optimizer but model2 was not converging, model3 designed
by ourselves with HeNormal initialisation converged slowly

# Conclusion:
We can conclude that CNNs are able to learn the entire task of lane and road following without manual decomposition into road or lane marking detection, semantic abstraction, path planning, and control.The 22 minutes of training data shows the car to operate in diverse conditions, on highways, local and residential roads in sunny and cloudy conditions. The CNN are able to learn meaningful road features from a very sparse training signal (steering alone).
Further work can be done to improve the robustness of the network by considering speed, brakes and gear system, we can also use augmentation to deal in extreme failure conditions , and to improve visualization of the network-internal processing steps.

# Team
* Mohammed Mohsin Ali (S20180010105), 
* Kandukuri Sai Teja (S20180010073), 
* Nikhil Kataria (S20180010118), 
* Bhavin Bansiwal (S20180010025).
