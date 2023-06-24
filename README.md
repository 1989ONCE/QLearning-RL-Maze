# QLearning-RL-Maze
Find 5 treasures and EXIT with minimum steps (QLearning)

### Map:
<img width="633" alt="Map" src="https://github.com/1989ONCE/QLearning-RL-Maze/assets/92381825/02acc310-ca9b-4495-8312-027715aba2e9">
  
  - wall positions: [4,5,7,9,22,23,25,30,31,35,39,43,45,47,49,50,51,53,55,57,58,59,61,65,71,74,80,85,88,90,94,97,100,101,102,104,109,110,111,113,114,119,120,127,128,129,132,134,136,141,142,143,145,151,153,155,157,158,164,166,169,172,176,178,181,183,186,187,190,191,193,195,196,206,211,214,226,229]
  - treasure positions: [6, 79, 170, 212, 227]
  - exit position : 230

### Settings:
- hyperparameters Setting
-> EPSILON = 0.9 (randomness of ACTIONS) </br>
-> ALPHA = 0.1 (learning-rate) </br>
-> GAMMA = 1 (desire for future rewards: 0 -> ignore future rewards, 1 -> look for high rewards in the long term) </br>
-> MAX_EPISODES = 1000 (amount of times of walking through the maze) </br>
- Reward Setting
-> goal_reward (exit found): 5000 </br>
-> wall_punish (hit into the wall): -300 </br>
-> out_punishment (go out of the map): -200 </br>
-> treasure_found: 1000</br>
-> normal_reward (normal path): -100</br>

### Best Result with no treasure found
Steps = 60 (at episode 442)</br>
Path: </br>
<img width="305" alt="no treasure best path" src="https://github.com/1989ONCE/QLearning-RL-Maze/assets/92381825/342c0e98-2aaf-4212-b20b-9f511863e719">

### Best Result with 5 treasure found
Steps = 501 (at episode 80)</br>
Path: </br>
<img width="305" alt="image" src="https://github.com/1989ONCE/QLearning-RL-Maze/assets/92381825/a90629c9-aa49-4935-8967-09c5a0378d2b">
