---
title: "大三（上）——微电路设计"
collection: publications
category: conferences
permalink: /publication/2025-10-microcircuit-design
excerpt: "以扫地机器人为载体的交叉项目驱动专业学科，涉及嵌入式软硬件（包含PCB设计，绘制，程序编写等），运动控制，激光雷达，导航算法，路径规划，上位机控制等一体化项目"
date: 2025-10-17
#venue: 'GitHub Journal of Bugs'
#paperurl: 'http://academicpages.github.io/files/paper3.pdf'
#citation: 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---

## Abstract
You can get more information just clicking here：[微电路设计报告]({{ site.baseurl }}/files/Microcircuit(5).pdf). 

<img src="{{ site.baseurl }}/images/Microcircuit(5).jpg" alt="Microcircuit(5)" style="display:block; margin:0 auto 1rem auto; max-width:100%; width:660px; height:auto;" />

This project presents the design and implementation of an **intelligent autonomous vacuum-cleaning robot (BY3D-Pro)** developed for the **Microcircuit Design** course. The system integrates **custom embedded hardware, real-time control firmware, wireless communication, and ROS2-based autonomous navigation** to realize a practical household cleaning robot with high precision, robustness, and interactivity.

The robot adopts a **heterogeneous and decoupled architecture** composed of an **x86 host running ROS2**, an **STM32F407 microcontroller** for hard real-time control, and **dual ESP32 coprocessors** for communication isolation. High-bandwidth LiDAR data and low-latency motion commands are transmitted on separate wireless links, preventing perception traffic from disturbing the motor control loop and ensuring deterministic control behavior.

For state estimation, **wheel encoders and a 9-axis IMU** are fused through a **tightly coupled Extended Kalman Filter (EKF)** to generate **low-drift, high-frequency odometry**, which provides reliable motion priors for SLAM. **Cartographer 2D SLAM** is used to build globally consistent maps via submap matching and pose-graph optimization with loop closure, while **AMCL with KLD-adaptive sampling** enables robust localization and recovery from localization loss.

Autonomous navigation is implemented using the **ROS2 Nav2 stack**. A customized **A*-based global planner** is combined with **minimum-snap polynomial trajectory optimization** to produce smooth, dynamically feasible paths. For cleaning tasks, a **coverage planner based on monotone polygon decomposition** generates systematic **boustrophedon (zig-zag) trajectories**, minimizing missed and repeated areas. A **TEB local planner** handles dynamic obstacles in real time, enabling smooth and safe navigation in household environments.

On the hardware side, the robot employs a **multi-domain power system** with a **14.4 V lithium battery**, high-current motor and fan rails, a **5 V buck stage**, and low-noise **3.3 V logic rails**. Motion is driven by **A4950 H-bridge drivers** with **1000 Hz PID closed-loop control** and **quadrature encoders**, achieving high straight-line accuracy and stable low-speed behavior. A fully redesigned **V2.0 PCB** improves grounding, EMI suppression, and thermal performance, significantly increasing current capacity and system reliability.

Overall, the project demonstrates a **full-stack robotic platform** that tightly couples **microcircuit design, embedded real-time control, and modern autonomous navigation algorithms**, delivering a vacuum robot capable of **accurate mapping, smooth motion, robust obstacle avoidance, and practical home deployment**.

------