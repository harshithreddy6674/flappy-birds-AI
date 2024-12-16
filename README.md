Flappy Bird AI 🐦🤖

This project demonstrates an AI trained to autonomously play the classic Flappy Bird game using NEAT (NeuroEvolution of Augmenting Topologies). The AI evolves neural networks to make intelligent decisions, like when to "flap" or stay still, optimizing its gameplay over generations.

🚀 Features

Game Simulation: The Flappy Bird game environment is recreated using PyGame.
AI Training: Utilizes the NEAT library to evolve neural networks for controlling the bird.
Dynamic Obstacles: Includes randomly generated pipes for realistic and challenging gameplay.
Fitness Evaluation: Assigns fitness scores to encourage progress and survival.
Visualization: Tracks generations and neural network performance.

📂 Project Structure

flappy_bird_ai.py: Main script containing game logic, NEAT integration, and training workflow.
config-feedforward.txt: Configuration file for NEAT parameters (population, mutation rates, etc.).
imgs/: Directory containing game assets (bird, pipes, background).
visualize.py: Optional module for visualizing NEAT neural networks and stats.

🛠️ Technologies Used

Python: Core programming language.
PyGame: Game development and environment simulation.
NEAT-Python: Neuroevolution library for training the AI.

📊 How It Works

Game Mechanics:

The bird must navigate through pipes by jumping or staying still.
Crashing into a pipe or the floor ends the game for that bird.
Neural Network Training:

Inputs: Bird's vertical position, distance to the next pipe, and pipe gaps.
Outputs: A single decision (whether to "flap" or not).
Fitness Function: Rewards survival time and progress through pipes.
Evolution:

Over generations, the NEAT algorithm improves the bird's decision-making.
High-performing networks are retained, while others mutate or recombine to explore new strategies.
