---
name: Trajectory Planning of Robot Arm using RL
tools: [Python, ROS, Open CV, Gazebo, MoveIt]
image: https://raviteja-kolli.github.io/assets/ur5_gif.gif
description: Reinforcement Learning-based control system for the UR5 Robotic Arm and optimizing the motion planning of the UR5 robotic arm using reinforcement learning techniques. By utilizing openai_ros, MoveIt, and advanced reinforcement learning algorithms, the robotic arm was trained to follow trajectories efficiently in a simulated environment.
---

<br>
### Brief overview
<br>
The UR5 is very easy to set up and program which gives one of the fastest payback times on the market. This robot can be operational in less than half a day thanks to the simple way of programming with a 3D visualisation. The robot can be moved manually to the right positions, after which it is stored and can be further adjusted on a touchscreen tablet.By using openai_ros, MoveIt, and advanced reinforcement learning algorithms, the robotic arm was trained to follow trajectories efficiently in a simulated environment. The work was executed using ROS and Python interfaces, with results visualized through RViz simulation. Future work aims at enhancing algorithms, optimizing training processes, and deploying the system on real hardware. 

### Hardware
UR5 Robotic Arm

Manufacturer: Universal Robots

Model: UR5

Carrying Capacity: 5 KG

Reach Radius: 850 mm

Applications: Packing, assembly, testing, and other light tasks.

### Software
Libraries and Packages Used:

* openai_ros:

Provides an interface for developing reinforcement learning environments in ROS. The Documentation can be found at: 
<p class="text-center">
{% include elements/button.html link="https://wiki.ros.org/openai_ros" text="openai_ros" %}
</p>

* MoveIt (Python Interface):

Offers a Python-based interface for performing tasks such as: Setting joint or pose goals, Creating motion plans, Moving the robot and adding, attaching, and detaching objects in the environment.

Documentation: Move Group Python Interface

The project pipeline includes three stages: 

**Stage 1 - Trajectory Planning Using Reinforcement Learning:**
<br>
The objective of this project was to train a robotic arm using reinforcement learning techniques to efficiently follow specified trajectories and achieve predetermined goals. To optimize the control actions of the robotic arm, policy-based methods such as PPO (Proximal Policy Optimization) and DDPG (Deep Deterministic Policy Gradient) were tested. The training process was conducted in a simulated environment using the openai_ros package, operating within a ROS infrastructure. Through this approach, the robotic arm learned by receiving reward signals based on successful trajectory completion and minimizing errors.
<br>
<img src="{{ site.url }}{{ site.baseurl }}/assets/gazebo_ur5.png"/>
<br>

**Stage 2 - Python Interface Control (MoveIt):**
<br>
The approach aimed at simplifying interaction with the robotic arm by setting up joint targets, defining pose goals, generating motion plans, and executing these planned paths through ROS communication channels, with the MoveIt library providing essential functions for smooth and collision-free path planning.
<br>
<br>
<img src="{{ site.url }}{{ site.baseurl }}/assets/control.png"/>
<br>

**Stage 3 - Environment Setup:**
<br>
The training environment for the reinforcement learning agent was established using the openai_ros package, incorporating ROS nodes for communication, custom-defined environments for task-specific learning, and enabling the agent to navigate and manipulate the robotic arm within a virtual simulation.
<br>
