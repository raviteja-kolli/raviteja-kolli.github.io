---
name: Autonomous Hexapod
tools: [MATLAB, Embedded Systems, Arduino]
image: https://raviteja-kolli.github.io/assets/Hexapod-in-Action.gif
description: This project aimed to develop a hexapod spider robot capable of performing walking and rotation gaits using a kinematic profile-based approach. By generating joint angles for each leg at each step, the robot was designed to achieve stable and efficient locomotion
---

# Bioinspired Hexapod for Adaptable Terrain Navigation
<br>
### Brief overview
<br>
The Hexapod Kinematics project focuses on designing and implementing a bio-inspired hexapod spider robot that emulates the movement of spiders. The motivation behind this project stems from the versatility, efficiency, adaptability, and stability of hexapod robots, which make them suitable for tasks requiring robust locomotion. The robot's design draws inspiration from the exoskeletons of insects and employs various gait optimization techniques.
<br>

### Hardware
* Microcontroller: Arduino (used for controlling servomotors)

* Motors: Three servo motors per leg (shoulder, elbow, and wrist)

* Power Supply: 5V power source for motors

* Wiring: Control pins connected to Arduino pins 9, 10, and 11

The mechatronics setup is as below:
<br>
<img src="{{ site.url }}{{ site.baseurl }}/assets/Mechatronics Setup.png" style="height: 300px; width:400px;"/>
<br>

### Software and Approach

* MATLAB: Used for simulation of motor orientations and generating kinematic profiles

* Arduino IDE & Tinkercad: Employed for coding and testing the single-leg setup

* CSV Files: Generated to store motor position data for validation


The Hexapod Kinematics project employed a combination of kinematic profiling, simulation, and benchtop testing to achieve stable and efficient locomotion.

The kinematic profiling method involved generating joint angles for each leg based on desired step parameters such as step length, step height, and walking speed. This approach was used to achieve two primary types of motion: walking gait and rotation without translation.

For the walking gait, a tripod gait was implemented where the robot moves three legs simultaneously while the other three provide support. This method ensures stability by alternating the active legs in a pattern where legs 1, 3, and 5 move first, followed by legs 2, 4, and 6. This creates a stable triangular base, allowing for effective locomotion with minimal risk of tipping over.

The rotation gait without translation was achieved by adjusting the positions and angles of the legs to coordinate movement around the central axis. By fine-tuning the phase difference between legs, the robot achieves smooth and stable rotation while keeping the body stationary. Adjustments to joint angles are made to ensure synchronized motion, maintaining balance and control throughout the rotation.

In addition to these motion techniques, the project utilized simulation tools to validate the effectiveness of the proposed gaits. MATLAB was employed to simulate motor orientations, allowing for comparison between simulated positions and actual motor angles. This helped ensure accuracy and consistency in the control mechanisms.

Benchtop testing further verified the kinematic profiles generated in simulation. During these tests, angles were adjusted iteratively to refine the robot's motion and ensure smooth operation. Testing of both the walking and rotation gaits provided valuable insights into the robot’s performance, including potential areas for improvement in control algorithms and surface interaction.
<br>
<img src="{{ site.url }}{{ site.baseurl }}/assets/Autonomous Hexapod.png"/>
<br>


### Results and Future Scope

The robot successfully performed both walking and rotational gaits, with field tests involving all six legs. While rotation demonstrated minimal deviation, walking presented lateral drift due to asymmetric leg movements and insufficient friction. Adjustments in angle signs helped achieve smoother motion. Performance plots indicated consistent leg-ground interactions but suggested a need for optimization in surface interaction and force distribution.

Future improvements include fine-tuning leg movements, enhancing surface interaction, and integrating sensors for real-time feedback. Adopting bioinspired locomotion techniques such as metachronal gaits could enhance future designs. Incorporating force/torque sensors, IMUs, vision sensors, and environmental sensors would increase the robot’s versatility and make it suitable for advanced applications in search and rescue, exploration, and agriculture.

<p class="text-center">
{% include elements/button.html link="https://github.com/raviteja-kolli/Autonomous_hexapod" text="Report" %}
</p>
