# Flappy Bird AI
This repository contains an implementation of a NEAT (NeuroEvolution of Augmenting Topologies) Python solution for playing the popular game Flappy Bird. The goal is to evolve a neural network that can successfully navigate through the pipes for as long as possible.

# Getting Started
These instructions will guide you on how to run the AI on your local machine.

# Prerequisites
You'll need to have Python installed, along with the Pygame and NEAT-Python libraries.
pip install pygame neat-python

# Running the Program
To run the program, simply clone the repository, navigate to its directory, and run the Python script.
python flappy_bird_neat.py

# Understanding the Code
The program leverages the NEAT algorithm to train a population of neural networks to play the game. It does this through a process of evolution, whereby networks that perform well are selectively bred over generations.

The Bird, Pipe, and Base classes represent the main elements of the game. The bird is controlled by the neural network, which decides when to jump based on its current position, velocity, and distance from the next pipe.

Each time a bird successfully navigates through a pipe, it is rewarded with an increase in fitness. If a bird hits a pipe, its fitness is decreased, and it is removed from the game. The game continues until all birds in the population have hit a pipe. The entire process is then repeated for a set number of generations.

# Important Note
The NEAT configuration parameters are stored in the config-feedforward.txt file, which should be located in the same directory as the script.

# Contributing
Please read CONTRIBUTING.md for details on our code of conduct, and the process for submitting pull requests to us.

# License
This project is licensed under the MIT License - see the LICENSE.md file for details.