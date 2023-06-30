# Traffic-Light-Management-Using-AI:-
Despite the fact that computer vision is today a highly developed field, capabilities for recognition and classification are not frequently used in day-to-day activities. Therefore, in this project we will make use of the current traffic infrastructure with some additional requirements, to create and demonstrate an advanced traffic light management.
# Abstract:-
Increasing traffic congestion at signalized junctions is a matter of great concern for creating and maintaining sustainable cities. Traffic jams in addition to adding to drivers' delays and stress levels, traffic bottlenecks significantly increase fuel usage and pollution. The main reason behind this is the way of controlling traffic at such junctions. Semi-automated and conventional traffic management has reached it’s saturation point and can no longer handle the high density of traffic flow with complex patterns. In this paper, we discuss and draw comparisons of previous research and works done to solve this problem. Our focus would be on techniques using Machine Learning, such as Computer Vision and Deep Neural Networks.
# Introduction :-
Numerous road networks are experiencing issues due to the decline in road capacity and the accompanying Level of Service as a result of the rise in automobiles in metropolitan areas. The bottleneck for these high vehicular flow are the conventional traffic management system used in these cities. There are two ways to tackle traffic flow currently in implementation : semi-automatic traffic lights with fixed timings or traffic police stationed at junctions to control the flow manually. The problem with use of traffic lights is that they use a fixed time for each side of the cross road, irrespective of the density of vehicles on those roads.

+ ![Traffic Signals](https://github.com/Nayeemhabib/Traffic-Light-Management-Using-AI/assets/117503421/441a445b-96d0-4deb-b2d3-630c8a08904c)
+ ![Traffic Signals](https://github.com/Nayeemhabib/Traffic-Light-Management-Using-AI/assets/117503421/7cd705be-4a0c-489b-9266-47357ce9c5d4)
  
Ideally, the road with higher density of vehicles should be given extra time to pass the junction, as that will lead to lower waiting time on average for all of the vehicles. Depending on manual control of traffic at junctions with manpower is inefficient, as a human cannot process all of the information at live with great accuracy for a longer time. Despite the fact that computer vision is today a highly developed field, capabilities for recognition and classification are not frequently used in day-to-day activities. Therefore, in this project we will be using Machine Vision to improve the current state of traffic. We would also come across some new methodology and techniques in analysis and decision making for traffic lights using live cameras installed at junctions
# Problem Statement:-
To build a self adaptive traffic light control system based on YOLO. Disproportionate and diverse traffic in different lanes leads to inefficient utilization of same time slot for each of them characterized by slower speeds, longer trip times, and increased vehicular queuing.To create a system which enable the traffic management system to take time allocation decisions for a particular lane according to the traffic density on other different lanes with the help of cameras, image processing modules.
# Methodology:-
+ The solution can be explained in four simple steps:-
   1. Get a real time image of each lane.
   2. Scan and determine traffic density.
   3. Input this data to the Time Allocation module.
   4. The output will be the time slots for each lane, accordingly.
+ ![yolo](https://github.com/Nayeemhabib/Traffic-Light-Management-Using-AI/assets/117503421/d6946201-3b45-42c7-bb11-aee7f9835556)
+ ![boy](https://github.com/Nayeemhabib/Traffic-Light-Management-Using-AI/assets/117503421/cb79580e-200a-4023-a2d9-951249a07bb1)
# Results and Discussion:-
+ The result for the project could be divided in two divisions:-
   1. Evaluation of Vehicle Detection Model The vehicle detection module was tested with a variety of test images containing varying amounts of vehicles, and the accuracy of detection was found to be in the range of 75-80%. Some test results are shown above in Fig. 3. This is satisfactory, but not optimum. The primary reason for low accuracy is the lack of a proper dataset. To improve upon this, real-life footage from traffic cameras can be used to train the model, so that accuracy of the system can be improved. We have used the images from the live feed camera installed at the traffic junctions or at normal traffic spots around the city or on the outskirts. These videos or live feeds were used to feed the model based on YOLO and OpenCV, where we detected the vehicle and there movement as in downwards or upwards, i.e., towards the traffic signal or away from it. We were also successful in defining what type of vehicle is it.
   + ![car](https://github.com/Nayeemhabib/Traffic-Light-Management-Using-AI/assets/117503421/4196073e-785a-47b9-83e1-30cc69ab6285)
   + ![car 2](https://github.com/Nayeemhabib/Traffic-Light-Management-Using-AI/assets/117503421/9a6c3f74-fc84-441d-8dac-45b39347991b)
We were also succesfull in implementing the derived traffic density from the detection module to the model for finding the optimum timings for each traffic lane to pass the vehicles. This was done on the principle of giving more priority or giving more time to the lane with higher traffic density and lesser to the ones with relatively uncrowded lane, while not creating bottlenecks or congestion in any one lane. For the same purpose, we created a simple simulation using PyGame.
  + ![end](https://github.com/Nayeemhabib/Traffic-Light-Management-Using-AI/assets/117503421/a7c45f00-03db-420c-a1a7-951c8e90540e)
  2. Evaluation of the Proposed Adaptive System For the pupose of evaluation of the system, the traffic movement simulation for both the system was run for 5 minutes a total of 15 times, using which the total number of vehicles that were able to pass through this junction were calculated



