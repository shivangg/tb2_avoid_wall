### Steps to Reproduce on the Robot Development Studios(RDS)

#### 1. Start the simulation of the Turtlebot2 (TB2) with a wall in front of it.

Go to the Simulations Tab and navigate to the TB2 simulation and start it.

#### 2. Open a terminal in the run the command

```
roslaunch tb_wall_avoider start_training_wall.launch
```

And you will see the robot start learning using Qlearning(RL).

### To run it on your own ROSject

#### 1. Start the simulation as suggusted above.

#### Install the tb_wall_avoider package

```sh
cd ~/catkin_ws/src
git clone https://github.com/shivangg/tb2_avoid_wall.git  # to clone this repo
cd ~/catkin_ws # catkin_make always run from this location
catkin_make #to compile the package 
source devel/setup.bash
roslaunch tb_wall_avoider start_training_wall.launch 
```
