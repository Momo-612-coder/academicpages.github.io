---
title: "College Students'Innovation Program"
excerpt: "Summarized some of the work content in the laboratory"
collection: portfolio
---

## Vision-Guided Precision Flight System

**National Undergraduate Innovation Training Program**  
You can click here to get more details[Report(PDF)]({{ site.baseurl }}/files/College_innovation.pdf). 

Principal Investigator: Xiangyu Mo  
Team Members: Dinghe Guo, Haowen Zheng, Weicheng Wang  
Supervisor: Chengliang Wang  

---

## Research Background

In emergency response scenarios such as vehicle fires, early-stage building fires, and hazardous material environments, traditional manual deployment of firefighting devices suffers from several limitations:

- low delivery accuracy  
- limited deployment range  
- high risk to personnel  

To address these challenges, this project investigates a **vision-guided precision flight system** capable of autonomous target detection and guided impact delivery.

We propose a **hierarchical guidance architecture** combining a **ground-based launcher guidance system** and an **onboard terminal correction mechanism**, enabling accurate target engagement with lightweight airborne hardware.

---

## Research Objectives

The project aims to develop a **miniature vision-guided flight system** with the following capabilities:

- visual target detection
- flight attitude control
- trajectory correction
- precision payload delivery

The system integrates:

- a launcher vision platform
- an embedded flight control system
- a guided projectile structure
- a coordinated control framework

---

## System Architecture

The system consists of two major subsystems:

### Launcher Guidance Platform

The launcher integrates:

- industrial camera
- NUC embedded computer
- OpenCV-based vision processing

Functions include:

- target detection
- target direction estimation
- launcher orientation control

A **two-axis gimbal (Yaw / Pitch)** adjusts the launch direction to minimize the initial trajectory error.

---

### Guided Flight Vehicle

The projectile integrates:

- STM32H743 flight controller
- IMU inertial sensor
- OpenMV embedded vision module
- servo control surfaces
- onboard power management system

The onboard system performs:

- attitude estimation
- visual target tracking
- flight trajectory correction

The onboard vision module performs **terminal guidance adjustments** during the descent phase.

---

### Launch Mechanism

The launcher uses a **high-speed friction wheel acceleration system**:

- DJI 3508 motors drive the friction wheels
- large inertia wheels ensure stable launch velocity
- four projectiles can be loaded simultaneously

The launcher platform provides:

- two-axis orientation control
- precision screw-drive positioning
- modular payload loading

---

## Research Process

The project follows a **system engineering methodology**, progressing through several development stages.

### Stage 1 – Requirement Analysis

- Investigation of current firefighting delivery methods
- Comparison of **laser, infrared, and vision guidance**
- Selection of **vision-based guidance**
- Development of the cooperative guidance architecture

---

### Stage 2 – Aerodynamic and Structural Design

Initial prototypes used a **fixed-wing configuration**, which showed insufficient stability.

The design was later replaced with an **X-tail configuration**, providing:

- improved aerodynamic stability
- independent control surfaces
- better trajectory control authority

Multiple prototype iterations were tested through simulation and experimental launches.

---

### Stage 3 – Embedded System Development

The embedded avionics system includes:

- STM32H743 flight controller
- OpenMV vision processor
- power management module
- multi-servo control system

Development tasks included:

- PCB design
- embedded software architecture
- flight control algorithm implementation

---

### Stage 4 – Integrated System Testing

Extensive experiments were conducted to evaluate:

- launcher stability
- projectile trajectory
- visual tracking performance
- launcher auto-aiming accuracy

The system was iteratively optimized based on experimental data.

---

## Key Innovations

### Hierarchical Vision Guidance Architecture

The project proposes a **two-layer guidance framework**:

- launcher performs coarse aiming
- projectile performs terminal guidance

This architecture significantly reduces onboard computational requirements.

---

### V-tail Mixing Flight Control Algorithm

A **V-tail mixing algorithm** is implemented:

- pitch, yaw, and roll are controlled using shared control surfaces
- control allocation matrix decouples the torques
- improves flight control responsiveness

---

### Highly Integrated Projectile Design

The projectile integrates all avionics into a compact body with a cross-section of:40 mm × 40 mm
Despite the limited space, the design accommodates:

- flight controller
- vision module
- power system
- actuator mechanisms

---

### Modular Launcher Platform

The launcher adopts a **modular design**:

- multi-projectile loading
- interchangeable payload module
- high repeatability launch mechanism

---

## Outcomes

The project successfully developed:

- guided projectile prototypes
- launcher control system
- vision tracking algorithms
- embedded flight control system
- integrated system testing platform

The results provide a practical engineering approach for **lightweight precision delivery systems**.

---
