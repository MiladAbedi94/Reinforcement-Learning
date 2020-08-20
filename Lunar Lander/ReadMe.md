# Deep Q Learning (Double Q-Learning)

In a 2015 paper titled ["Deep Reinforcement Learning with Double Q-learning"](https://arxiv.org/abs/1509.06461) by  Google Deep Mind researchers, the authors presented a very interesting, yet simple and effective upgrade upon the traditional Deep Q Learning. The approach presented in this paper, helped greatly reduce the problem of over-estimation of Q values that inflicted the existing Deep Q Learning methods in the Atari Games domain.

In short, the authors proposed retaining two separate Deep Q Networks (DQN), online and offline, as opposed to one. This allows us to choose actions based on one of the DQN's whilst evaluating the action based on the other. While the paper suggests a delayed update to the offline network by directly copying the weights of the online network, I have found it more effective to perform soft updates on the offline network towards the online network.

The implementation of the agent can be found in the [Jypyter Notebook file](DQN%20Lunar%20Lander.ipynb). A report of the project (introduction + hyper parameter tuning + results and discussion) can be found in the [PDF file](Deep%20Q%20Learning.pdf).


# Results:



After 10 Episodes

<img src="./Videos/After%2010.gif" width="500"/>
After 200 Episodes

<img src="./Videos/After%20200.gif" width="500"/>
After 400 Episodes

<img src="./Videos/After%20400.gif" width="500"/>
After 600 Episodes

<img src="./Videos/After%20600.gif" width="500"/>
After 800 Episodes

<img src="./Videos/After%20800.gif" width="500"/>
After 1000 Episodes

<img src="./Videos/After%201000.gif" width="500"/>
After 2000 Episodes

<img src="./Videos/After%202000.gif" width="500"/>