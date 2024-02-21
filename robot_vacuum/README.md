# Reflex Based Vacuum Cleaner Agent

## About this Project

The goal of this project is to build a reflex agent vacuum that can navigate through a room while cleaning the dirty parts of the room. The agent is unaware of its environment. It can only react based off of its percepts.

## Data & Dependencies

My implementation of this project takes place in Jupyter Notebook and utilizes helper functions given by the professor.

## Technical Approach

I first implement the simulation environment. Next, I implement a simple reflex agent. This agent has no sense of state, therefore, it can only randomly walk around and react to its sensors. Then, I implement a model-based reflex agent. This agent first moves to a corner of the room, and then the agent snakes through the room and cleans the dirty squares. 

After I build the two agents, I compare their performances using simulation. Furthermore, I use boxplots, line charts, and tables to visualize my results.

Finally, I implement an environment that includes obstacles. Again, I analyze the performance of my agents.

## Highlights

* Model based agents
* Simple reflex agents
* Visual analysis

## Conclusion

As the size of the room increases, the disparity between the performance of the different models also increases. For n = 5, the random agent has the worst performance followed by the simple reflex agent and then the model-based agent. As the size of the room increases, this difference becomes larger and larger. At size n = 10 and size n = 100, the random agent and simple reflex agents reach the max number of steps for every run. Meanwhile, the model-based agent takes an average of 128.64 and 12045.01 respectively.

