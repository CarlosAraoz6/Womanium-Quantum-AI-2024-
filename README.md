### Womanium-Quantum-AI-2024-

# Quantum Solutions for the Poisson Equation: Implementing the HHL Algorithm
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

**Slide Presentation (PDF Format):** A comprehensive presentation outlining our approach, methodology, and results. The slide presentation is named **"QuantumPoissonSolver-Slides.pdf"** and covers the theoretical background, implementation steps, and conclusions drawn from the project. Link: https://github.com/CarlosAraoz6/Womanium-Quantum-AI-2024-/blob/main/QuantumPoissonSolver-Slides.pdf

### Jupyter Notebookk "Quantum_AI_for_Climate final.ipynb" : https://github.com/CarlosAraoz6/Womanium-Quantum-AI-2024-/blob/main/Quantum_AI_for_Climate%20final.ipynb
#### 1. Problem Statement and Background

The first section of the Jupyter notebook addresses the problem statement and background for the project. It provides a detailed explanation of the Poisson equation, a fundamental partial differential equation (PDE) used in various scientific and engineering fields. The section highlights the significance of the Poisson equation in modeling static fields and its applications in areas such as groundwater flow simulation, weather prediction, photovoltaic cell optimization, and carbon sequestration.

Readers will find an exploration of why solving the Poisson equation is crucial for advancing these applications, particularly in the context of resource management, clean energy, and climate change mitigation. The notebook also explains the relevance of this problem to the broader goals of the Womanium Quantum+AI 2024 Hackathon and why it is an interesting and impactful challenge to tackle using quantum computing techniques.

This section sets the stage for the subsequent technical work by grounding the project in a clear and compelling real-world context.


#### 2. Background Research and Literature Review

The second section of the Jupyter notebook delves into the classical methods traditionally used to solve the Poisson equation. This part provides a concise yet comprehensive review of the different techniques that have been developed and refined over time to address the computational challenges associated with solving this fundamental partial differential equation.

Readers will find descriptions of key classical approaches, including:

+ Finite Difference Method (FDM).

+ Finite Element Method (FEM).

+ Multigrid Methods.

+ Spectral Methods.

The section also highlights the challenges and limitations of these classical methods, particularly in terms of computational complexity and resource demands, especially as problem sizes increase. This underscores the need to explore alternative approaches, such as quantum computing and AI/ML techniques, to advance the field.

References to relevant literature are provided throughout this section, offering readers further insights into the development and application of these classical methods.





#### 3. AI/ML and Quantum Computing Techniques

The third section of the Jupyter notebook explores how AI/ML and quantum computing techniques can be applied to solve the Poisson equation, highlighting recent advancements and their potential to overcome the limitations of classical methods.

This section includes:

+ Quantum Computing Approaches.

+ Harrow, Hassidim, and Lloyd (HHL) Algorithm.

+ Variational Quantum Algorithms (VQAs).

+ Quantum Algorithm for NISQ Devices.

+ Comparative Analysis.

+ Computational Resources.

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
