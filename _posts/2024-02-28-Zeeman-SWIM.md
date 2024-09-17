---
title : "Paper summary: Global biasing using a hardware-based artificial Zeeman term in spinwave Ising machines"
layout : single
author_profile : true
---

In this post, I’d like to give an overview of my latest research, **"Global biasing using a hardware-based artificial Zeeman term in spinwave Ising machines."** This work takes a closer look at **spinwave Ising machines (SWIMs)** and how we can push their complexity by introducing a global bias using an artificial Zeeman term.

### What is a Spinwave Ising Machine?

A **spinwave Ising machine (SWIM)** is a device designed to solve complex combinatorial optimization problems, which fall under the class of NP-hard problems. It uses propagating spinwave RF pulses in materials like Yttrium-Iron-Garnet (YIG) to map out solutions in a physical system. SWIMs rely on **phase-sensitive amplification (PSA)** to generate binary spin states—basically, tiny "units" that mimic spins in a physical system. These spins can then represent solutions to difficult problems like the traveling salesman or knapsack problem.

### Key Insights from the Paper

1. **Introducing Global Biasing:**
   In this study, we took the standard SWIM and added a **global biasing** feature using an external microwave signal. This external signal, known as an **artificial Zeeman term,** aligns the spins in a preferred direction, making the system behave like it’s under the influence of a magnetic field. This technique enhances the mathematical complexity of the SWIM, allowing it to tackle more challenging optimization tasks.

2. **The Role of the Zeeman Term:**
   By applying a continuous external signal at the same frequency as the spinwave RF pulses, we introduced a **Zeeman term** to the system. This term biases the spins so that they align in a certain direction, despite the usual antiferromagnetic coupling (where neighboring spins prefer to point in opposite directions). The result is **ferromagnetic ordering**, which helps the system find more complex solutions to problems.

3. **Amplifying the Complexity:**
   With the addition of this Zeeman term, the SWIM is now able to handle more complicated problem sets. We tested this by adjusting the amplitude and phase of the external signal, which effectively changed the way the artificial spins behaved. The introduction of global bias not only allowed us to manipulate the system into ferromagnetic states but also led to the emergence of unexpected mixed spin states (like 3 spins up and 1 spin down) when certain parameters were met.

4. **Exploring New States:**
   One of the more interesting findings was that intermediate values of the Zeeman signal created a **phase transition** in the system, resulting in these **3+1 states.** Although these states weren’t part of the system’s minimum energy solution, they offered a fascinating glimpse into the complexities that arise when dealing with nonlinear amplification and phase-shifted signals. We traced this behavior back to the limitations in the low-noise amplifier (LNA), which can saturate and cause uneven amplification.

5. **Applications for the Future:**
   This research opens up new possibilities for enhancing the **spinwave Ising machine** to solve even more complex combinatorial problems. By adding the Zeeman term, we’ve expanded the range of problems the system can tackle, while also introducing the potential for further complexity through phase transitions. In future iterations, we could improve the system’s performance by refining the amplification process or even integrating digital feedback systems like FPGAs to stabilize the spin states.

### Wrapping Up

Overall, this work is a step forward in developing more powerful hardware-based solvers for optimization problems. The ability to introduce global biasing through an artificial Zeeman term gives the spinwave Ising machine a new level of versatility. While we uncovered some unexpected behaviors (like the 3+1 spin states), these offer valuable insights into how we can further refine the system. I’m excited to see how this technology can evolve and continue pushing the boundaries of **unconventional computation.**

If you’re into the nitty-gritty details of spintronics and optimization, this project demonstrates how adding a simple external signal can dramatically change the behavior of complex systems like SWIMs. The future of hardware-based solvers looks bright, and I can’t wait to see where this path takes us next.

[Link to the paper](https://doi.org/10.1063/5.0185888)
