# Grain growth modelling
Simple application written in python to showcase cellular automatons. 
It uses very naive approach of drawing grid of squares and to see how the system would change over time.
You can read about them more [here](https://en.wikipedia.org/wiki/Cellular_automaton).

## update 

新增double分支，为双层焊缝的模拟，possible分支计算了晶粒生长的方向概率，db_heat为打底焊的晶粒之间竞争生长的情况

# Features
* Allows for different grid sizes
* Supported neighbourhoods: [Moore](https://en.wikipedia.org/wiki/Moore_neighborhood), [Von Neumann](https://en.wikipedia.org/wiki/Von_Neumann_neighborhood), Hexagonal Left/Right, Random Hexagonal and Random Pentagonal.
* Periodical and non periodical neighbourhoods (meaning they can or cannot cross over border).
* Initialize system with: random grains on random positions, evenly distributed or randomized with specified radius.
* Ability to pause and start on a whim.

# Example gif!
<p align="center">
  <img width="600" height="400" src="https://media.giphy.com/media/chzxShioR2Msc0RE3H/giphy.gif">
</p>

# Installation and running
This does require some additional libraries so if you don't have them  you can simply install them by running:
```
pip install -r requirements.txt
```
To run use:
```
python main.py
```

# Last words

It can crash if you desire to open up more than 1 grid window at the time. You can close and create new one but it is currently not possible to have two at once.
The limitation sadly comes from the pygame library which is used to draw said grid as it can have only one context window at once.
Feel free to download the code and play with it however you like. Don't expect too much of it:)
