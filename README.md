**Written by Rupesh Mahore , IISc Bangalore**
# Locust Swarm Simulation
This Python code simulates the behavior of a swarm of locusts using the agent-based model. The simulation is a two-dimensional grid in which the agents move according to the rules defined by the model.

# Dependencies
The following Python packages are required to run the simulation:

* numpy
* matplotlib
* matplotlib.animation


# Simulation Parameters
The following simulation parameters can be customized by changing the corresponding values in the code:

* n_agents: Number of locust agents
* grid_size: Size of the simulation grid
* time_steps: Number of simulation time steps
* neighborhood_size: Size of the locust's local neighborhood
* marching_threshold: Threshold for determining if a locust will march
* band_threshold: Threshold for determining if a locust will form a band

For each locust, a decision is made whether to march in a random direction or form a band and move towards the closest locust in their neighborhood, based on the **marching_threshold** and **band_threshold parameters**. If the locust decides to march, its orientation is set to a random direction within a certain range of its neighbors' average orientation. If the locust decides to form a band, its orientation is set to the orientation of the closest locust in its neighborhood. The locust's position is then updated by moving in the direction of its new orientation, with periodic boundary conditions enforced to keep the locusts within the simulation grid.

# Running the Simulation
To run the simulation, simply execute the Python code in your preferred environment or terminal. The resulting animation will be saved as a video file named **'locusts.mp4'** in the same directory as the code file.

# Animation
The animation shows the movement of the locust swarm over time. Each locust is represented by an arrow that indicates its current orientation, and the color of the arrow indicates the locust's current movement state. Black arrows indicate locusts that are stationary, red arrows indicate locusts that are moving towards their neighbors, and blue arrows indicate locusts that are moving in a random direction.
