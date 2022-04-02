# Folk-Fulkerson algorithm to solve the maximum flow problem in a railway network system.
* Written by: [Ivy Wu S.Y.](https://www.linkedin.com/in/ivy-wusumyi)
* Technologies: VBA, user form, Folk-Fulkerson algorithm, optimsation


## 1. Introduction
Maximum flow problem is a common optimasation problem within a flow network. This project is aimed at developing a user friendly decision making model for the railway industry by telling how many trains per day can be sent from a chosen origin station to a chosen destination, as well as the number of trains can be run on each rail segment. As such, the Ford-Fulkerson algorithm is used to calculate the maximum amount of flow within a railway network by  analyzing the capacity of each railway segment and produce a result of maximum flow for each route. 


## 2. Methodology & Solution
The solver uses the Ford-Fulkerson algorithm to calculate the optimal flows of each railway segment. The idea of the algorithm is to detect any rail segments with available capacity connecting from the origin station to the destination while sending flow along with the segments until no more segments can be found. In other words, the algorithm loops all the possible rail segments until all capacities are used up eventually. The outputs of the Ford-Fulkerson algorithm are divided into 2 parts, optimal flows and journeys. The optimal flow output is a summarized table for all possible rail segments and their respective flows and capacities information. Users can easily know how many trains per segment can be sent to reach the maximum flow from the origin to the destination. On the contrary, the journey output contains a detailed version of flow information and their respective capacities per each journey. Users can hence further understand the network flow and find the bottleneck of capacity for further improvements.<br/>
<img src="/images/flow.png?raw=true" width="550">


## 3. User Interfaces
To increase the usability of the solver, two interactive user forms are built to provide guidance and allow easier data input. Users could navigate on the main tab to initiate functions for different purposes.<br/>
<img src="/images/tab.png?raw=true" width="250">

### 3.1 Define Problem Size
The user form contains 3 parts sequentially from “Clear Data”, “Problem Size” to “Station Linkage Data”. The proposed user journey is designed to start from top to bottom, in which users should first clear the existing data before starting a new problem and subsequently define the stations and input rail segment data. <br/>
<img src="/images/define_problem.png?raw=true" width="550">

### 3.2 Define Origin and Destination
The second user form is created for users to initiate the Ford-Fulkerson algorithm. Two dropdown lists of stations are retrieved dynamically for users to select their origin station and the desired destination. The solve button will call the program to run the algorithm and generate outputs. <br/>
<img src="/images/solver.png?raw=true" width="400">

### 3.3 Sample Output
Summary output of optimal flows from the Oxford station to the Gatwick Airport station.<br/>
<img src="/images/summary.png?raw=true" width="550"><br/>

Datiled journey of optimal flows from the Oxford station to the Gatwick Airport station.<br/>
<img src="/images/journey.png?raw=true" width="550"><br/>


## 4. About the programming

### 4.1 Files
The solver is developed in an Excel with VBA and user forms embedded. The solver is available [here](/Railway_maximum_flow_solver.xlsm).

### 4.2 Data
A sample station list of the British train operating company, Great Western Railway, is provided in the XLSM file.

### To learn more about Ivy Wu S.Y., visit her [LinkedIn profile](https://www.linkedin.com/in/ivy-wusumyi)

All rights reserved 2022. All codes are developed and owned by Ivy Wu S.Y..