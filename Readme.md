# Reinforcement Learning
Reinforcement learning (RL) is an area of machine learning concerned with how intelligent agents ought to take actions in an environment in order to maximize the notion of cumulative reward.
In this game our agent snake considers food as reward and the snake learns through reinforcement learning and understands the environment.

## How to run
Run these 2 queries in anaconda prompt/python cmd

1. To activate and set the environment
	-conda activate pygame_env (Make sure pygame lib is installed)

2. To run the game
	-python agent.py


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
