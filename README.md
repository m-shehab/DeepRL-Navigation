# DeepRL-Navigation
"Navigate and collect" Agent. Udacity Deep Reinforcement Learning Nanodegree 1st Project.

## Project overview 
In this project we implement a reinforcement learning agent using [Deep Q-Networks](https://deepmind.com/research/dqn/). The agent is required to learn the how to navigate in a 2D world and collect bananas in the given environment. The bananas in the environment is divided into yellow banans to be collected to get a reward, and blue bananas to be skipped to avoid punishments. The 2D world environment, where the agent navigates, is based on [Unity ML-agents](https://github.com/Unity-Technologies/ml-agents) and the environment looks as in the figure below.

![img_1](Figures/navigation.gif)

## Environment details 
The state space of the given environment consists of 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. The agent is supposed to take an action based on receiving this information. 
The action space consisits of four discrete actions as indicated below: 
- 0 - move forward.
- 1 - move backward.
- 2 - turn left.
- 3 - turn right.

To learn the optimal policy, a reward of +1 is provided for collecting a yellow banana, and a reward of -1 (i.e. a punishment) is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.

**Note:** The project environment provided by Udacity is similar to, but not identical to the [Banana Collector](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#banana-collector) environment on the Unity ML-Agents GitHub page.

## Installation and Running 

1. Configure a Python 3.6 / PyTorch 0.4.0 environment with the needed requirements as described in the [Udacity repository](https://github.com/udacity/deep-reinforcement-learning#dependencies)

2. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

3. Download the `Naviagtion.ipynb`, `model.py` and `dqn_agent.py` files in the DeepRL-Navigation GitHub repository and make them accessible to your python environment. 

## Training 
Execute the provided notebook within Deep Reinforcement Learning Udacity online workspace for navigation project after modifying `Naviagtion.ipynb` and related files. 
