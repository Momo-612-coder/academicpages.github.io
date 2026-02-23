---
title: "大三（上）——数学物理方法"
collection: publications
category: conferences
permalink: /publication/2025-10-mathematicsphysic
excerpt: "本文系统研究了 FDM 3D 打印层状材料在不同打印角度下的应力与应变分布特征及断裂机理，通过理论建模、数值求解、有限元仿真与三点弯曲实验验证打印角度对结构承载能力和局部应变集中的影响规律。"
date: 2025-10-17
#venue: 'GitHub Journal of Bugs'
#paperurl: 'http://academicpages.github.io/files/paper3.pdf'
#citation: 'Your Name, You. (2024). &quot;Paper Title Number 3.&quot; <i>GitHub Journal of Bugs</i>. 1(3).'
---

## Abstract
You can get more information just clicking here：[数学物理方法-3D打印层状应力分析]({{ site.baseurl }}/files/Method-of-mathematicsphysic(5).pdf).

<img src="{{ site.baseurl }}/images/Method-of-mathematicsphysic(5).jpg" alt="Method-of-mathematicsphysic(5)" style="display:block; margin:0 auto 1rem auto; max-width:100%; width:660px; height:auto;" />

This study systematically investigates the **strain distribution** and **stress concentration** characteristics of **Fused Deposition Modeling (FDM) 3D printed layered materials** under varying **raster angles**. The work focuses on **PLA beams** subjected to **three-point bending**, combining **theoretical modeling**, **numerical solution**, **finite element simulation**, and **experimental validation** to analyze the influence of **print orientation** on structural load capacity and failure mechanisms.

At the theoretical level, a **multi-layered beam stress field model** is established using **two-dimensional elasticity** and **Airy stress functions**. **Fourier series expansion** is employed to derive an analytical solution, while **orthotropic assumptions** and the **Tsai-Hill failure criterion** are applied to predict theoretical failure stress for different printing angles.

Numerically, a **MATLAB program** based on the **finite difference method** is developed to solve the **biharmonic equation**, enabling visualization of **stress and strain fields**, and validating the theoretical model within the elastic regime. At the simulation level, **explicit dynamic analysis** using **ANSYS/LS-DYNA** captures stress-strain evolution under both **small and large displacement loading conditions**, reflecting the layered structure’s mechanical response.

Experimental **three-point bending tests** confirm the theoretical and simulation predictions. Results show that in **small displacement loading**, stress distribution is largely governed by overall stiffness, and **equivalent stress** decreases slowly with increasing **raster angle**. In the **large deformation and fracture regime**, **maximum principal strain** is highly sensitive to **print orientation**: higher angles significantly amplify **local tensile strain concentration**, governing crack initiation and propagation.

Overall, the study demonstrates a **non-linear influence** of raster angle on mechanical performance. Minor deviations from the **ideal printing direction** result in limited strength variation, while angles beyond a **critical threshold** drastically reduce **interlayer load transfer** and overall structural capacity. The integrated theoretical, numerical, simulation, and experimental approach elucidates the mechanical essence of **orientation effects** in FDM printed components, providing a reliable foundation for **raster angle optimization** and structural design in engineering applications.

------