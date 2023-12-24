## NeuralEvolution-Self-Driving

Thıs repository is documented and cleaned version of my old project I did back in 2019 which can be found [here](https://github.com/berkealgul/DeepLearning-stuff/tree/master/self-driving)
and it is a toy project for me to learn about neural networks and evolutionary algorithms

The Project is about the implementation of deep neuralevolution algorithm and driving autonomous agents on different types of parkours.
Agents have laserscan sensors that casts rays around its surrounding and get distance mesaruments. These distance values and agents velocity and orientation information is given to the network.
As an output we get acceleration and steering changes that agents need to do
As the reward system checkpoints(blue dots) are used

<!--
[![IMAGE ALT TEXT](http://img.youtube.com/vi/iCH4GV00-2k/0.jpg)](https://www.youtube.com/watch?v=iCH4GV00-2k "Click to youtube") 
-->

<img src="https://github.com/berkealgul/NeuralEvolution-Self-Driving/blob/main/sim.gif" width="600" height="324"/>

### Features
- Custom neural network
- Genetic algorithm implementations
- Map editor tool

### How to use

#### Main simulation
You can run "main.py" to launch the simulation. 

The script uses "/mapData.json" for getting map information and "/bestcar.json" for getting and saving model parameters

There are several example parkours in "/parkours" folder. In order to use them, you can carry the desider json file to project directory and rename the file to "mapData.json"

Similarly you can use pretrained model in "/train models" directory, just rename it to "bestcar.json"

#### Map Generation Tool

Aside of already generated maps you can also create and edit your own custom maps. In order to do that you can run "MapTools/mapMain.py" file. 
With that editor you can place walls, determine start/finish point and adding checkpoints. The map is going to saved when you exit the application

Maps you created are saved in "/mapData.json" file, dont forget to extract that file

If you want to create an empty map from scratch you can replace "/mapData.json" file with "MapTools/emptyMap.json"

<b>Note</b> : Checkpoints cant be deleted and you need to place them in order from start to finish of the parkour
