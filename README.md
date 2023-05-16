# Using Mixed Integer Programming to solve supply-demand mismatch for bike sharing service

Public bike sharing services often face an unbalanced distribution of bikes among the stations across the city. As users tend to follow specific destination flows when going to work, school, or other daily activities (mainly moving from residential areas to downtown in the morning, and vice-versa in the afternoon), many
stations with a high demand for bikes end up being full, which stops other users from being able to dock their bicycles at their destination.)

The final objective was to develop a model which suggests the optimal bike relocating strategy around the city, and consequently allowing more customers to utilize the service. In order to do so, a linear optimization model was built which relocates bikes from stations with lower demand to stations observing relatively higher demands.

The following two datasets were used to develop the linear optimization problem:
1. A dataset with all the stations' infromation, including station’s ID, name, longitude, latitude, and total bike capacity
2. A dataset with information about trips observed in the 3rd quarter of 2017 including the trip ID, the initial and final station id, as well as the trip duration, date, and time.

Gurobi - a mathematical programming package was used in python to formulate and solve this problem. Due to the complicated nature of the problem, multiple simlifying assumptions were made to ensure the functionality of the model. 

The project was also supported by a sensitivity analysis to investigate the impact of changing demand or prices.


<p align="center">
  <img width="830" height="350" src="https://github.com/codebyvictor/Rebalancing-Optimization-for-Bike-sharing-Systems/blob/15670d71cd9794acd85617ffafdb47f9dd938617/bixi.png">
</p>
