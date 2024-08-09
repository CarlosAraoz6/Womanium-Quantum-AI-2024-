### Womanium-Quantum-AI-2024-

# Quantum Poisson Equation Solver with HHL Algorithm
### Womanium Quantum Hackathon 2024

### Team: QAI Climate MX

Team Members

Name: Carlos Aráoz Alvarado

Discord ID: 733107032454070292

Discord User: Carlos Aráoz#5582

Github User: CarlosAraoz6

Contact Email: caa.ppbt90@gmail.com



## Challenge Title: Quantum Solutions for the Poisson Equation: Implementing the HHL Algorithm

### Challenge Description:

In this project, we implemented the Harrow-Hassidim-Lloyd (HHL) algorithm to solve the Poisson equation, leveraging the power of quantum computing to address this fundamental partial differential equation. The Poisson equation plays a significant role in various scientific and engineering applications, making it an excellent candidate for demonstrating the advantages of quantum algorithms over classical methods.

Project Deliverables:
Our solution includes the following elements:

Slide Presentation (PDF Format): A comprehensive presentation outlining our approach, methodology, and results. The slide presentation is named "QuantumPoissonSolver-Slides.pdf" and covers the theoretical background, implementation steps, and conclusions drawn from the project.

### Jupyter Notebookk "Quantum_AI_for_Climate final.ipynb" :
#### 1. Problem Statement and Background

The first section of the Jupyter notebook addresses the problem statement and background for the project. It provides a detailed explanation of the Poisson equation, a fundamental partial differential equation (PDE) used in various scientific and engineering fields. The section highlights the significance of the Poisson equation in modeling static fields and its applications in areas such as groundwater flow simulation, weather prediction, photovoltaic cell optimization, and carbon sequestration.

Readers will find an exploration of why solving the Poisson equation is crucial for advancing these applications, particularly in the context of resource management, clean energy, and climate change mitigation. The notebook also explains the relevance of this problem to the broader goals of the Womanium Quantum+AI 2024 Hackathon and why it is an interesting and impactful challenge to tackle using quantum computing techniques.

This section sets the stage for the subsequent technical work by grounding the project in a clear and compelling real-world context.


#### 2. Background Research and Literature Review

The second section of the Jupyter notebook delves into the classical methods traditionally used to solve the Poisson equation. This part provides a concise yet comprehensive review of the different techniques that have been developed and refined over time to address the computational challenges associated with solving this fundamental partial differential equation.

Readers will find descriptions of key classical approaches, including:

+ Finite Difference Method (FDM): A straightforward method that converts the PDE into a system of algebraic equations using difference equations. It is effective for simple geometries but becomes computationally intensive for large-scale problems.

+ Finite Element Method (FEM): A versatile technique that divides the domain into smaller sub-domains (elements) and uses test functions to convert the PDE into algebraic equations. It handles complex geometries more effectively but requires more sophisticated implementation and computational resources.

+ Multigrid Methods: These methods accelerate the convergence of iterative solvers by solving the problem on a hierarchy of grids. They offer fast convergence for large-scale problems but have complex implementations that require careful parameter tuning.

+ Spectral Methods: These represent the solution as a sum of basis functions and are highly accurate for smooth solutions. However, they may struggle with complex geometries and discontinuities.

The section also highlights the challenges and limitations of these classical methods, particularly in terms of computational complexity and resource demands, especially as problem sizes increase. This underscores the need to explore alternative approaches, such as quantum computing and AI/ML techniques, to advance the field.

References to relevant literature are provided throughout this section, offering readers further insights into the development and application of these classical methods.





#### 3. AI/ML and Quantum Computing Techniques

The third section of the Jupyter notebook explores how AI/ML and quantum computing techniques can be applied to solve the Poisson equation, highlighting recent advancements and their potential to overcome the limitations of classical methods.

This section includes:

+ Quantum Computing Approaches: An overview of how quantum computing has been leveraged to reduce the computational costs associated with solving partial differential equations (PDEs) like the Poisson equation. The section details how quantum simulations have been used in semiconductor physics, particularly in analyzing gate insulators, demonstrating the advantages of quantum parallelism.

+ Harrow, Hassidim, and Lloyd (HHL) Algorithm: A significant focus is placed on the HHL algorithm, which is designed to solve systems of linear equations exponentially faster than classical methods under certain conditions. The notebook explains how the HHL algorithm can be applied to solve the Poisson equation by discretizing it into a sparse matrix form and using quantum operations to find the solution.

+ Variational Quantum Algorithms (VQAs): The section also covers VQAs, hybrid algorithms that combine quantum and classical computing resources to solve optimization problems. Examples include the Variational Quantum Eigensolver (VQE) and the Quantum Approximate Optimization Algorithm (QAOA), which have been successfully applied to solve the Poisson equation.

+ Quantum Algorithm for NISQ Devices: The discussion includes algorithms developed for noisy intermediate-scale quantum (NISQ) devices, which are current quantum computers with limited qubits and error correction capabilities. The section highlights the importance of constructing quantum algorithms that can be implemented on these devices to perform meaningful computations.

+ Comparative Analysis: The advantages and disadvantages of quantum algorithms compared to classical methods are discussed. While classical methods like FDM, FEM, and Multigrid Methods are well-understood and effective for small problems, they face challenges with scalability and computational efficiency. Quantum algorithms, such as HHL and VQAs, offer significant speedups for large-scale problems but are currently limited by hardware constraints.

+ Computational Resources: The section also details the computational resources required to implement these quantum algorithms, including the need for access to quantum computing hardware, sufficient qubits, and classical optimization techniques for parameter adjustment in VQAs.

This section provides a comprehensive view of the cutting-edge techniques in quantum computing that hold the potential to revolutionize the way we solve the Poisson equation and similar PDEs.

#### 4. Methodology: AI/Quantum Methods
   
In the fourth section of the Jupyter notebook, we present the implementation of the Harrow, Hassidim, and Lloyd (HHL) algorithm to solve the Poisson equation, a crucial partial differential equation (PDE) with wide-ranging applications in science and engineering. This section walks through the design and execution of a quantum circuit that leverages the HHL algorithm to obtain a solution to the Poisson equation.

This section includes:

Quantum Circuit Design:

+ State Initialization: The quantum circuit begins by initializing a quantum state that corresponds to the normalized vector b. This is done using the initialize_b function, which sets up the initial quantum state.

+ Application of Gates: Hadamard gates are applied to all qubits, creating a superposition state. The circuit then applies controlled-unitary operations corresponding to the matrix A, which represents the discretized Laplacian operator.

+ Quantum Phase Estimation: The Quantum Fourier Transform (QFT) is applied to estimate the eigenvalues of A, followed by the Inverse Quantum Fourier Transform (IQFT) to revert the state back to the computational basis.

+ Measurement: The final step is measuring the ancillary qubit to obtain the solution to the Poisson equation.
  
#### Execution and Simulation:

The quantum circuit is executed on a quantum simulator (AerSimulator) to simulate the behavior of a quantum computer. The execution involves transpiling the circuit and running it with a noise model to simulate real-world quantum conditions.
Output Analysis: The results of the execution are presented as a histogram of measurement counts, showing the frequency of the ancillary qubit being measured in states 0 and 1. The obtained counts indicate how the quantum algorithm processes the Poisson equation solution.
Code Implementation: The notebook provides the complete code used for the implementation, including functions for circuit creation, execution on a simulator, and result visualization.

This section showcases the practical application of quantum computing techniques to solve the Poisson equation and demonstrates the capabilities of the HHL algorithm in this context. It also offers insights into the potential of quantum algorithms to address complex PDEs that are computationally intensive for classical methods.


#### Discussion
The implementation of the HHL algorithm to solve the Poisson equation in this project produced promising results. The ancillary qubit was measured in state 0 approximately 75% of the time, indicating that the algorithm effectively approximated the solution. The presence of noise, simulated through a depolarizing error model, resulted in a 25% occurrence of state 1, reflecting the algorithm's sensitivity to noise.

#### Conclusion
The HHL algorithm successfully demonstrated its capability to solve the Poisson equation on a quantum simulator, with the majority of measurements aligning with the expected solution. Despite the impact of noise, the results confirm the algorithm's potential in quantum computing applications, particularly for solving complex partial differential equations. Future work could focus on mitigating noise effects and scaling the algorithm to more qubits for broader applicability.



#### Additional Notes

Some files may need to be downloaded to view them correctly.


#### Submission Details

Repository Link: https://github.com/CarlosAraoz6/Womanium-Quantum-AI-2024-/tree/main

Submission Deadline: August 9, 2024, 23:59pm US ET
