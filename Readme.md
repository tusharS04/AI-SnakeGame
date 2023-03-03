# Reinforcement Learning
Reinforcement learning (RL) is an area of machine learning concerned with how intelligent agents ought to take actions in an environment in order to maximize the notion of cumulative reward.
In this game our agent snake considers food as reward and the snake learns through reinforcement learning and understands the environment.

## How to run

### To run the game Follow the instructions 
Run all the queries in anaconda prompt/python cmd

> Make sure you have conda, pygame and torchvision modules installed (pip install module_name)

> You must have created an environment 
> If not then you can create  one by the following command
	``` conda create -n pygame_env python=3.7 ```

> To activate and set the environment
	``` conda activate pygame_env ```

> To run the game
	``` python agent.py ```


## Working

### Agent:
- game
- model

### Training:
- State = get_state(game)
- action = get_mov(state)
	- model.predict()
- reward, game_over, score = game.play_step(action)
- new_state = get_state(game)
- remember -> model.train()

### Game (Pygame):
- play_step(action)
	-> reward, game_over, score
	
### Model (PyTorch):
-Linear_QNet(DQN)
-model.predict(state) -> action
