---
title: "大三（上）——自动控制"
collection: publications
category: conferences
permalink: /publication/2025-10-auto-control
excerpt: "本报告基于连续导通模式下 Buck 变换器的小信号建模与频域分析方法，结合 PI 闭环控制策略与 STM32 数字实现，对直流稳压电源的稳定性、动态性能及寄生参数影响进行了系统研究，并完成创意智能台灯控制系统的工程实现。"
date: 2025-10-17
#venue: 'GitHub Journal of Bugs'
#paperurl: 'http://academicpages.github.io/files/paper3.pdf'
#citation: 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---

## Abstract

## Detailed Abstract

This course project presents the design, modeling, analysis, and implementation of a DC regulated power supply based on a Buck converter, followed by the development of an intelligent desk lamp control system as an integrated application. The work is conducted within the framework of classical control theory, combining power electronics with feedback control principles.

The Buck converter operates in **Continuous Conduction Mode (CCM)** with a 24 V DC input and a nominal 12 V output (adjustable from 10 V to 12 V), delivering up to 2 A load current. A small-signal averaged model is derived using linearization around the steady-state operating point. The control-to-output transfer function is obtained, representing the power stage as a second-order system dominated by the LC output filter dynamics. The resulting mathematical model serves as the foundation for controller design and frequency-domain analysis.

System stability and dynamic performance are systematically analyzed using classical control tools, including the **Routh–Hurwitz stability criterion**, **root locus method**, **Nyquist stability criterion**, and **Bode plot analysis**. The effects of passive component parasitics—particularly the **equivalent series resistance (ESR)** of the output capacitor—are incorporated into the model. It is shown that ESR introduces an additional zero, significantly influencing phase margin and high-frequency behavior. Both theoretical calculations and **PSIM simulations** validate the necessity of including parasitic parameters for accurate high-frequency modeling.

A closed-loop voltage control strategy is implemented using an **STM32 microcontroller**. The output voltage is sampled through an ADC channel, conditioned via signal amplification and filtering circuits, and regulated using a discrete **PI controller**. The controller adjusts the PWM duty cycle to achieve stable voltage regulation. Experimental results demonstrate that under a 24 V input, the system maintains a stable 12 V output with steady-state error within ±1%, output ripple below 100 mV (typically around 72 mV peak-to-peak), and satisfactory dynamic response under load transients and reference voltage step changes between 10 V and 12 V. The closed-loop system exhibits adequate phase margin and robustness against parameter variations.

Based on the stabilized DC power platform, the project further extends to the implementation of a **creative intelligent desk lamp system**. The system integrates ambient light sensing, manual dimming control, and display interfaces. A multi-modal control strategy and state-machine logic are designed to ensure smooth brightness tracking and flicker-free operation. The control system demonstrates fast command tracking and stable output regulation during brightness transitions, enhancing user experience.

Overall, this project follows a complete engineering workflow—**modeling, analysis, simulation, hardware implementation, and experimental verification**—bridging theoretical control concepts with practical power electronics applications. It validates the effectiveness of classical linear control theory in the design and optimization of switching power supply systems.

You can get more information just clicking here：[BUCK控制实现报告]({{ site.baseurl }}/files/Automatic-control(5).pdf). 
------