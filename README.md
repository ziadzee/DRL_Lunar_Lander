# Reinforcement Learning Implementations

- Implemented a Q-Learning algorithm on Grid World `environment` in which an `agent` (mouse) navigates her grid `environment` collecting `rewards` (cheese) with the goal of escaping the environment. The `agent` has the `actions` of `Up`, `Down`, `Left` and `Right` which allows her to move between `states`.

- Implemented the Soft Actor-Critic model proposed by Haarnoja et al., (2018) to Open AI's Lunar Lander problem. 

- Implemented and carried out a comparative performance of Double DQN, Dueling DQN and Prioritised DQN for solving Lunar Lander problem.


# Packages

- Python Version: `3.8.11`

- Libraries and Packages: `numpy` , `pandas`, `seaborn`, `operator`, `torch`, `gym`, `plotly` , `random` , `collections`


# Outcomes

### Q-Learning Grid World
- For our Q-Learning algorithmL, the random policy performs poorly and in an unpredictiable manner as expected:

![image](https://user-images.githubusercontent.com/65977822/133047100-c089c6b4-6419-4a93-a554-0167eae4cc2e.png)

- For different values for `Alpha` (learning rate) , `Gamma` (the discount factor) and `Epsilon` (action selection):

![image](https://user-images.githubusercontent.com/65977822/133047853-590b76fc-7a66-4d66-91fd-3acaac5cecf7.png)

![image](https://user-images.githubusercontent.com/65977822/133047888-d16d1071-d568-441a-94be-682f21bb7f69.png)

![image](https://user-images.githubusercontent.com/65977822/133047913-d4b19aea-b5f8-4b51-a72c-03f529ff2daf.png)


### Soft Actor-Critic (Deep Reinforcement Learning)

- We found that the Soft Actor-Critic didn't perform very well in our implementation for the Lunar Lander problem. The agent behaved in a very stochastic manner and failed to adequately learn the rules of the game after many epochs:

![image](https://user-images.githubusercontent.com/65977822/133048289-63ee4bcb-50cc-426a-9f45-4f96dc821cab.png)


### Double DQN, Dueling DQN and Prioritised DQN (Deep Reinforcement Learning)

- Lastly, out of the three DQN models the Prioritised DQN model performed best when considering the loss function. It is interesting to note that all three models achieved negative rewards across all epochs:

![image](https://user-images.githubusercontent.com/65977822/133049123-00f0fc3e-6426-4eeb-88f4-a2d49d3223a3.png)

# Specifications

Code and outcomes for the above can be found in the follow Jupyter notebooks:

- Q-Learning Grid World: `Q_Learning_Grid_World`
- Soft Actor-Critic: `Soft_Actor_Critic`
- Double DQN, Dueling DQN and Prioritised DQN: `DQN_comparison`

For more information regarding Lunar Lander and OpenAI, see https://gym.openai.com/envs/LunarLander-v2/
