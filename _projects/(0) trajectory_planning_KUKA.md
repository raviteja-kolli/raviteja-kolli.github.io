---
name: KUKA Robot Trajectory Planning
tools: [MATLAB, Robotics System Toolbox]
image: https://raviteja-kolli.github.io/assets/project3.jpg
description: The primary objective is to program the robot to position a rectangular shape accurately on a rectangular target within its workspace. Leveraging an Aruco marker for target detection, the robotic arm uses a camera mounted on its flange to determine the target’s location and orientation.
---

# Efficient robotic motion planning for industrial automation
<br>
### Objective
<br>
This project explores the precise control and motion planning capabilities of the KUKA LBR iiwa 7 R800 robotic arm, focusing on real-world applications of robotics in dynamic environments. The primary objective is to program the robot to position a rectangular shape accurately on a rectangular target within its workspace. Leveraging an Aruco marker for target detection, the robotic arm uses a camera mounted on its flange to determine the target’s location and orientation. The trajectory planning, executed in joint space, ensures compliance with joint constraints and achieves the desired motion with precision in exactly 10 seconds. This project demonstrates the potential of robotics in precision tasks, offering insights into advanced motion planning and real-time adaptability.
Inspired by the increasing demand for precision in robotics, this project incorporated modern control techniques and efficient kinematic modeling to achieve seamless and reliable trajectory planning.
<br>
<br>
**My Focus**: The project involved the development of trajectory planning algorithms for a 7-DOF robotic arm:
Kinematic Modeling: Forward and inverse kinematics equations were derived to model the robot's movements accurately.
Trajectory Planning: Polynomial interpolation and linear segment blending techniques were used to design smooth joint-space trajectories.
Execution Time: A 10-second time frame was optimized for point-to-point motion tasks, balancing precision and speed.
Simulation Tools: MATLAB Robotics Toolbox for trajectory generation and visualization.
<br><br>
**Results**: Achieved precise point-to-point motion within a 10-second time frame and validated smooth trajectory execution with MATLAB simulations.
<br>

### Arm Simulation
<br>
<img src="{{ site.url }}{{ site.baseurl }}/assets/project3 simulation.jpeg"/>
<br>

<br>
### Future Scope 
* Real-Time Adaptability: Incorporate sensor feedback to dynamically adjust trajectories in real time.
* AI Integration: Use machine learning for predictive motion planning.
* Industrial Applications: Extend to complex tasks like welding and assembly line automation.
