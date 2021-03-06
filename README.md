<h1> Udacity Deep Reinforcement Learning Nanodegree</h1>
  
<h2>Navigation Project</h2>

<h3>1. Project Description</h3>

The current project attempts to solve a task using a value-based model-free and off-policy deep reinforcement learning algorithm that uses a neural network to decide on which actions to take in its environment.

The task consists of an agent that needs to navigate a large square world and learn how to more around in order to catch the maximum number of yellow bananas while avoiding blue bananas. The environment provides a reward of +1 at each time-step if the agent catches a yellow banana and a punishment of -1 if the agent catches a blue banana. 

The goal of the agent is therefore to learn the locations of yellow bananas and move itself to those locations during the available time-steps in a given episode so as to maximise its total episodic reward.

<h3>2. Environment</h3>

An adapted version of the Banana Collector environment available in Unity ML-Agents GitHub page is used in this project. Observation states are composed of 37 variables which correspond to the agent’s velocity as well as a ray-based perception of objects located immediately in front of the agent. 

The action space is composed of 4 discrete actions corresponding to the direction that the agent has to move in the current time-step given its velocity and ray-based perception provided by the environment in the previous time-step which should give the agent an idea of where it is currently located. The available actions are 0 - move forward, 1 - move backward, 2 - turn left, 3 - turn right.

The task is of an episodic nature and the agent must learn how to map velocities and ray-based information to one of the discrete actions available in order to maximise its total reward during each episode. To solve the task, the agent must obtain an average score of +13 over 100 consecutive episodes.

<h3>3. Implementation</h3>

Our implementation uses makes use of a Q-network which we train using several techniques such as Fixed Q-targets, Double Q-learning, Duelling Networks and Priotitised Replay Buffer.

We also experiment with different hyper-parameters and loss functions such as Mean-Squared-Error and Huber-loss.

<h3>4. Running the Code</h3>
To run the code simply download the available files to a folder, open the Jupyter Notebook and select "Kernel -> Restart & Run All".

<h3>5. Dependencies</h3>
Python 3.6, Numpy 1.15.1, Pytorch 0.4.0, UnityEnvironment.

<h3>6. Credits</h3>
Finally we would also like to acknowledge the quality of the code and resources made available here: https://github.com/higgsfield which greatly accelerated the understanding of PyTorch and the different algorithms used in this project. 
Simply amazing work!
