# CS-370
Pirate intelligent agent that uses deep Q-learning and neural networks to navigate a treasure maze. CS 370 portfolio project.
## What work did I do on this project?

For this project, I worked on a pirate intelligent agent that learns to navigate a maze and reach the treasure using deep Q-learning. I was given a starter notebook, the TreasureMaze class for the environment, and the GameExperience class for experience replay. The starter notebook also included supporting code for displaying the maze, building the neural network, and evaluating the agent.

My main contribution was completing the qtrain() training algorithm. I added the logic to start games from random open cells, choose between exploration and exploitation, perform actions, and store experiences. I connected replay batches to the neural network training step, tracked wins and losses, updated the target network, and reduced exploration as training progressed. The saved run reached its stopping condition at epoch 293 and passed the completion check for every starting cell.

## What do computer scientists do, and why does it matter?

Computer scientists solve problems by designing, building, and testing programs and systems. They choose approaches based on the problem and use evidence to determine whether their solutions work. Their work matters because software can help people complete tasks, understand information, and make decisions.

This project helped me understand how a system can learn from feedback instead of having every action programmed in advance. The pirate learned navigation decisions through rewards and repeated experience. Similar ideas can be applied to areas such as robotics and automated planning, although those applications require more testing and safeguards than a maze game.

## How do I approach a problem as a computer scientist?

I start by understanding the goal, the requirements, and the code or tools already available. For this project, I needed to understand how the maze represented states, which actions the pirate could take, and how rewards affected learning. I broke the training process into smaller steps and checked how the environment, replay memory, and neural network worked together.

I also learned to look beyond one successful result. A recent 100% win rate alone did not prove the agent could win from every starting position, so the completion check was important. In future projects, I would continue breaking problems into smaller parts, testing assumptions, and checking results against the original requirements.

## What are my ethical responsibilities to the end user and the organization?

I am responsible for being honest about what a system can do, testing it carefully, and explaining its limitations. My agent succeeded on the maze used during training, but that does not prove it could solve an unfamiliar maze or always find the shortest route. I should not present those results as capabilities that were never tested.

For systems used by people or organizations, I also have a responsibility to protect private information, consider unfair or harmful outcomes, and provide appropriate human oversight. In reinforcement learning, the reward system needs careful attention because an agent may learn behavior that earns rewards without meeting the intended goal. Clear documentation and accurate reporting help users and organizations decide whether a system is appropriate for their needs.
