---
title: "College Students'Innovation Program"
excerpt: "Summarized some of the work content in the laboratory"
collection: portfolio
---
 
## Vision-Guided Precision Flight System  

You can click here to get more details：[Report(PDF)]({{ site.baseurl }}/files/College_innovation.pdf).   

**Project Type:** National Undergraduate Innovation and Entrepreneurship Training Program  
**Project Role:** Project Leader & Electrical Control System Developer  
**Institution:** Chongqing University  
**Advisor:** Prof. Chengliang Wang  
**Project Duration:** Oct 2024 – Dec 2025  

---

# 1. Research Background

Accurate delivery of payloads in hazardous environments such as early-stage warehouse fires or confined industrial spaces requires **high-precision targeting and rapid deployment mechanisms**.

Traditional solutions often rely on manual throwing devices or bulky robotic platforms, which suffer from:

- limited deployment distance
- low targeting accuracy
- high operational cost

To address these challenges, this project proposes a **vision-guided precision flight system** integrating:

- target detection
- launch platform alignment
- guided flight control
- payload delivery

The system enables autonomous targeting and launch of lightweight guided flying objects for precision strike or payload deployment.

The proposed architecture combines **mechanical launch systems, embedded control systems, and visual perception modules** into a unified robotic system. :contentReference[oaicite:0]{index=0}

---

# 2. System Architecture

The complete system consists of two main subsystems:

### Launch Platform

Responsible for:

- visual target detection
- orientation adjustment
- controlled launch

Key components include:

- Industrial camera + edge computer
- Yaw–Pitch two-axis pointing mechanism
- Friction-wheel launch module
- Embedded control system

The platform automatically detects target direction and aligns the launcher before releasing the guided vehicle. :contentReference[oaicite:1]{index=1}

---

### Guided Flight Vehicle

The guided vehicle integrates:

- onboard camera
- IMU sensors
- flight control processor
- control surfaces and actuators

Within a compact internal volume, the vehicle integrates sensing, control and payload modules while maintaining flight stability. :contentReference[oaicite:2]{index=2}

---

# 3. Hardware and Mechanical Design

### Launch Mechanism

After evaluating several candidate mechanisms including:

- spring launch
- electromagnetic launch
- friction wheel launch

the system adopted a **dual friction wheel launch mechanism** due to its:

- lower mechanical shock
- higher repeatability
- stable initial velocity

Experiments show that when the wheel speed reaches **4000 rpm**, the vehicle can achieve a flight range of approximately **20 meters**. :contentReference[oaicite:3]{index=3}

---

### Structural Design

Several engineering optimizations were implemented:

- cross-roller bearing yaw support to improve structural rigidity
- ball screw + linear rail mechanisms for precise pointing
- large-diameter friction wheels to reduce acceleration shock

These optimizations significantly improved launch consistency and system reliability. :contentReference[oaicite:4]{index=4}

---

# 4. Visual Perception and Target Detection

The launch platform uses a **monocular camera system** combined with computer vision algorithms.

The detection pipeline includes:

1. Gaussian filtering for noise reduction  
2. HSV color-space threshold segmentation  
3. Morphological filtering  
4. Connected component analysis for target extraction  

Target direction is estimated and transmitted to the launch controller at **50 Hz** for real-time alignment. :contentReference[oaicite:5]{index=5}

---

# 5. Flight Control and Guidance Algorithm

The onboard flight control system adopts a **multi-loop control architecture**.

### Sensor Fusion

The system fuses data from:

- onboard camera
- IMU (JY901)
- visual target offset measurements

Pixel coordinates from the camera frame are transformed into the world coordinate system using a rotation matrix while compensating for roll and pitch motion. :contentReference[oaicite:6]{index=6}

---

### Control Strategy

The flight control algorithm includes:

- attitude stabilization using PID / PD control
- rate-limited command smoothing
- roll compensation to reduce visual error
- visual guidance based on line-of-sight tracking

These algorithms ensure stable flight while maintaining target tracking capability.

---

# 6. Embedded System Design

The electrical system adopts a **distributed architecture** consisting of three boards:

- main flight controller
- vision processing module
- power management board

The system is designed around **STM32H743 embedded processors** and integrates multiple sensors and actuators within a highly constrained internal space. :contentReference[oaicite:7]{index=7}

To reduce payload weight and energy consumption, computationally intensive visual tasks are offloaded to the ground station. :contentReference[oaicite:8]{index=8}

---

# 7. Experimental Validation

Multiple rounds of system testing were conducted, including:

- wind tunnel experiments
- launch platform calibration
- real-world flight testing
- multi-cycle launch reliability testing

Key experimental findings include:

- launch speed variation < 3%  
- stable flight control after launch  
- reliable target alignment and delivery

The system maintained structural integrity after **over 2000 launch cycles**. :contentReference[oaicite:9]{index=9}

---

# 8. My Research Contributions

As the **project leader**, my responsibilities focused on system-level engineering and embedded control implementation.

My main contributions include:

- designing the electrical architecture of the guided flight vehicle
- developing embedded control firmware for flight stabilization
- integrating IMU sensors, camera modules, and control actuators
- implementing visual-guided flight control algorithms
- coordinating launch platform and vehicle control interaction
- organizing system-level testing and performance evaluation

Through this project, I developed strong capabilities in **robotic system integration, embedded control design, and experimental validation**.

---

# 9. Research Significance

This project demonstrates a low-cost and modular solution for **vision-guided precision delivery systems**.

The proposed system architecture highlights the importance of **co-design between mechanical systems, control algorithms, and perception modules**.

The work provides practical experience in:

- robotics system engineering
- autonomous guidance systems
- embedded flight control development

---

**Keywords:** Robotics, Vision Guidance, Autonomous Systems, Flight Control, Embedded Systems