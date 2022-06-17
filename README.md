## NeuralEvolution-Self-Driving

This project is about implementation of deep neuroevolution algorithm and driving autonomous agents on different types of parkours
Agents have laserscan sensors that casts rays around its surrounding and get distance mesaruments. These distance values and agents velocity and orientation information is given to the network.
As an output we get acceleration and steering changes that agents need to do
As the reward system checkpoints(blue dots) are used

### Features
- Custom neural network
- Genetic algorithm implementations
- Parkour editor

### How to use
You can run "main.py" to launch the simulation. 

The script uses "/mapData.json" for getting map information and "/bestcar.json" for getting and saving model parameters

There are several example parkours in "/parkours" folder. In order to use them, you can carry the desider json file to project directory and rename the file to "mapData.json" In addition you can also create your own maps

Similarly you can use pretrained model in "/train models" directory, just rename it to "bestcar.json"

