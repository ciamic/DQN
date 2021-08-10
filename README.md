# DQN
 Implementation of a generic Deep Q Network algorithm.
 
## Introduction
This repo contains: 
- an implementation of a DQN algorithm 
- a solution to the [Udacity Deep Reinforcement Learning Nanodegree](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893 "Udacity Deep Reinforcement Learning Nanodegree") Project 1, Navigation

### Project details

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

For this project, an agent has been trainied with the DQN algorithm in order to navigate (and collect bananas!) in a large, square world.

![Trained Agent][image1]

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and in order to consider the environment solved, the agent must get an average score of +13 over 100 consecutive episodes.

### Getting Started

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
	
	
2. Place the file in the repository folder, and unzip (or decompress) the file.

### Dependencies

To set up your python environment to run the code in this repository, follow the instructions below.

1. Create (and activate) a new environment with Python 3.6.

	- __Linux__ or __Mac__: 
	```bash
	conda create --name dqn python=3.6
	source activate dqn
	```
	- __Windows__: 
	```bash
	conda create --name dqn python=3.6 
	activate dqn
	```

3. Clone the repository, and then, install the required packages (see requirements).
```bash
git clone https://github.com/ciamic/DQN.git
```

4. Create an [IPython kernel](http://ipython.readthedocs.io/en/stable/install/kernel_install.html) for the `dqn` environment.  
```bash
python -m ipykernel install --user --name dqn --display-name "dqn"
```

5. Before running code in a notebook, change the kernel to match the `dqn` environment by using the drop-down contextual `Kernel` menu. 

### Requirements

- `Python 3`
- `Torch (v0.4)`
- `unityagents`
- `numpy`
- `matplotlib`

### Instructions

Follow the instructions in `Navigation.ipynb` to get started evaluating the agent, or train one from scratch!


### Ideas for Future Work

- Implement a [Double DQN](https://arxiv.org/abs/1509.06461 "Double DQN")
- Implement a [Dueling DQN](https://arxiv.org/abs/1511.06581 "Dueling DQN")
- Implement [Prioritized Experience Replay](https://arxiv.org/abs/1511.05952 "Prioritized Experience Replay")
- Implement [Rainbow](https://arxiv.org/abs/1710.02298 "Rainbow") extensions
- Learn directly from pixels as input (however, this would require a different environment)
