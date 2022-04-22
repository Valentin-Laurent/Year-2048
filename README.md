# Introduction
Here we train agents to play the game 2048 using reinforcement learning, thanks to the [Tensorforce library](https://github.com/tensorforce/tensorforce). The code has been pushed during an intense 2 weeks-long project, so this repo could use some cleaning (I've started working on it) :)

See the [main training notebook](https://github.com/Valentin-Laurent/Year-2048/blob/master/notebooks/Training_notebook.ipynb) for a nice overview of our work. You can also watch the demo of our project in [this video](https://youtu.be/MuwEa2A6XLA?t=1423), where I give an introduction to RL and an analysis of our results (8 minutes, in french).

We trained our best agent using [Deep Q-Learning](https://www.nature.com/articles/nature14236). It reaches the 1024 tile in about half of the games it plays, and the 2048 tile every 20 games or so.

# Set up
Clone this repository and install the dependencies (you may want to create a virtualenv first):
```bash
git clone git@github.com:Valentin-Laurent/Year-2048.git
cd Year-2048
pip install -r requirements.txt
```

# Quickstart
You can use the [main training notebook](https://github.com/Valentin-Laurent/Year-2048/blob/master/notebooks/Training_notebook.ipynb) to train an agent on your own. The agent params, metrics, and the agent itself will be saved in the `notebooks/data` folder. A single file will store all the training and testing metrics of all of your agents, and a single file will store the params of all of your agents. However, one folder per agent will be created in order to dump it.

You can also load existing agents to further train them, possibly with different params. A dump of our best agent is available for you in the `best_agent` folder!

Feel free to have a look at our other notebooks in `notebooks/drafts`. Please note that [we forked the gym-2048 environnement](https://github.com/Valentin-Laurent/gym-2048) to experiment on allowing illegal moves, modifying the reward, and more.
