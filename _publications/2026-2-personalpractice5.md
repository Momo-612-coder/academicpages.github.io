---
title: "个性化实践-大三（上）"
collection: publications
category: manuscripts
permalink: /publication/2026-2-personalpractice5
excerpt: "用于展示在大三（上）学期所有课外实践，包括无人机技术实验室研究，创新/创业实践，竞赛等等"
date: 2026.2
#venue: 'Journal 1'
#slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
#paperurl: 'http://momo-612-coder.github.io/academicpages.github.io/files/personal_practice_5.pdf'
#bibtexurl: 'http://academicpages.github.io/files/bibtex1.bib'
#citation: '莫湘渝, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---
## Abstract

This work documents a project-driven and system-level engineering practice carried out during the third-year personalized track in the Mingyue Innovation Class at Chongqing University.  
Instead of focusing on isolated technical modules, the work emphasizes how real engineering systems are defined, built, and iteratively validated under constraints of reliability, integration, and application scenarios.

The core technical component is the FT580 tandem-rotor heavy-lift UAV platform.  
Within this project, a complete avionics and electrical architecture was designed and implemented around PX4 and DroneCAN, including multi-node real-time communication, redundant power and control links, and safety-critical actuator management.  
A self-developed electrical control unit was built to bridge the flight controller and propulsion system, supporting engine control, power distribution, cooling, fuel pumping, and sensor acquisition, with quantified system-level performance such as millisecond-level command latency, low packet loss under multi-node load, and hardware-level over-current protection and redundancy.

To support system observability and safety, a high-current voltage-current-power sensing node was independently developed and iterated multiple times, providing real-time feedback and forming a reusable template for distributed UAV sensor networks.

Beyond laboratory UAV research, this work also includes a hardware-driven AI companion product for pet emotional interaction, in which embedded electronics and control systems were used to convert abstract emotional design goals into physically deployable interaction prototypes.  
Through motion modeling, servo control, and emotion-action mapping, a functional Demo 0.0 was realized and validated through real user studies.

In addition, a national-level innovation project on a vision-guided high-speed flight system was led to completion, covering flight dynamics, vision-based guidance, payload-carrying design, and system-level validation in real environments.  
The project achieved a fully integrated closed-loop system from launcher to guided vehicle, with documented hardware, control algorithms, communication protocols, and test results.

Overall, this work demonstrates a transition from component-level implementation to system-level engineering: starting from requirements, shaping architectures, implementing hardware and software, and validating complete robotic and aerial systems under realistic constraints.  
It establishes a reusable engineering methodology for UAVs and intelligent hardware that bridges research, prototyping, and deployable systems.

You can get more information just clicking here：[个性化实践5]({{ site.baseurl }}/files/personal_practice_5.pdf). 
------