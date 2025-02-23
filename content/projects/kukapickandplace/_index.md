---
title: Pick and Place with a Kuka Robot Arm
toc: false
cascade: 
    type: blog
---


### Introduction
During our labs in ECE470: Robot Modeling and Control, my classmates and I tackled motion planning and obstacle avoidance using the KUKA robotic arm. Our goal was to have the KUKA robotic arm pick up an object and drop it into a cup while avoiding obstacles. We utilized an artificial potential field (APF) algorithm, which combines attractive forces (pulling the arm toward its goal) and repulsive forces (pushing it away from obstacles). The lab also gave us the opportunity to experiment with different parameters and refine our algorithm to handle real-world complexities.


### Approach
The robot followed a predefined trajectory, ensuring it avoided obstacles and successfully grasped the object. Using inverse kinematics, we calculated the necessary joint angles and tested our motion plan in simulation before applying it to the physical robot. Using Matlab, we tested our repulsive function to ensure it generated the expected values.
{{< video src="armsim.mp4" muted="true" autoplay="true" loop="true">}}


### Demo
{{< video src="demo.mp4"  width="400px" muted="true" autoplay="true" loop="true">}}


