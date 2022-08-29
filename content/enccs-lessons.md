# ENCCS lessons

## GPU computing

### [OpenMP for GPU Offloading](https://enccs.github.io/openmp-gpu/miniapp/)

Learning objectives:
- Get an overview of the architecture of GPU and how they differ from CPUs
- Understand how OpenMP fits into the landscape of GPU programming approaches
- Understand OpenMP's shared parallel model and program execution model
- Learn how to use basic OpenMP directives and clauses

### [OpenACC](https://enccs.github.io/OpenACC/)

Learning objectives:
- Get an overview of the architecture of GPU and how they differ from CPUs
- Understand how OpenACC fits into the landscape of GPU programming approaches
- Understand OpenACC's shared parallel model and program execution model
- Learn how to use basic OpenACC directives and clauses

### [Intermediate CUDA](https://enccs.github.io/CUDA/)

Learning objectives:
- Get an overview of the architecture of GPU and how they differ from CPUs
- Understand GPU concepts like threads, blocks and streaming multiprocessors 
- Learn to write simple CUDA kernels
- Learn to work with GPU memory
- Learn to optimize CUDA kernels
- Understand asynchronous execution

### [SYCL](https://enccs.github.io/sycl-workshop/)

Learning objectives:
- What is SYCL and why it is useful.
- Write hardware-agnostic code to express parallelism using the queue, command group, and kernel abstractions.
- Use buffer and accessors to handle memory across devices.
- Evaluate drawbacks and advantages of unified shared memory.
- Get acquainted with the SYCL profiling API.

## HPC

### [Intermediate MPI](https://enccs.github.io/intermediate-mpi/)

Learning objectives:
- Understand communicators, groups and derived datatypes
- Learn to use one-sided communication
- Understand and be able to use collective communication, blocking and non-blocking
- Understand how to work with MPI and threads

## Programming languages

### [High-performance Data Analytics with Python](https://enccs.github.io/HPDA-Python/)

Learning objectives:
- Have a good overview of available tools and libraries for improving performance in Python
- Know what libraries are available for efficiently storing, reading and writing large data
- Be comfortable working with NumPy arrays and Pandas dataframes
- Be able to explain why Python code is often slow
- Understand the concept of vectorisation
- Understand the importance of measuring performance and profiling code before optimising
- Be able to describe the difference between “embarrasing”, shared-memory and distributed-memory parallelism
- Know the basics of parallel workflows, multiprocessing, multithreading and MPI
- Understand pre-compilation and know basic usage of Numba and Cython
- Have a mental model of how Dask achieves parallelism
- Remember key hardware differences between CPUs and GPUs
- Be able to create simple GPU kernels with Numba

### [Julia for High Performance Scientific Computing](https://enccs.github.io/Julia-for-HPC/)

Learning objectives:
- Experienced practioners in other languages understand what's different/special about Julia
- Become familiar with typical structure of a Julia package
- Set up efficient workflow for developing in Julia and using the package manager
- Learn to efficiently work with data 
- Know what performance pitfalls exist and learn to benchmark and profile code
- Learn to use multithreading and distributed computing
- Understand what different approaches exist for porting code to GPUs

## AI

### [Upscaling A.I. training](https://enccs.github.io/upscalingAItraining/)

Learning objectives:
- Learn different strategies to perform distributed training in TensorFlow
- Learn how to use Horovod for distributed training
- Learn to containerise neural network training

### [A.I. as a Tool for Change](https://www.youtube.com/watch?v=_FMnopQNF3M)

Learning objectives:
- Get an overview of possible use cases for artificial intelligence
- Understand how AI can effectively be put to use in different sectors and application domains
 

### [Graph Neural Networks and Transformer](https://enccs.github.io/gnn_transformers/)

Learning objectives:
- Learn to use graph neural networks
- Learn to use transformers



## Applications

### [Gromacs GPU Performance](https://enccs.github.io/gromacs-gpu-performance/)

Learning objectives:
- Understand the difference between MPI ranks and OpenMP threads when running GROMACS
- Be able to name the most important parts of the molecular dynamics workflow
- Appreciate some of the internal architecture of mdrun
- Know how to assign the PME workload
- Know how to use several GPUs efficiently.
- Know common pitfalls to avoid


### [VeloxChem: Quantum chemistry from laptop to HPC](https://enccs.github.io/veloxchem-workshop/)

Learning objectives:
- Learn to perform quantum chemical simulations of ground- and excited-state properties of large systems using VeloxChem.
- Leverage the aggregate resources of modern HPC clusters to efficiently tackle large molecular systems.
- Use the Python application programming interface (API) to prototype new methods.
- Design interactive computational teaching materials in Python.

 
### [OpenFOAM](https://enccs.github.io/OpenFOAM/)

Learning objectives:
- Learn how to use OpenFOAM



## Other

### [CMake](https://enccs.github.io/cmake-workshop/)

Learning objectives:
- 1
- 2

### [Containers](https://enccs.github.io/Containers/)

Learning objectives:
- Learn to use Docker
- Learn to use Singularity

#### [Introduction to Quantum Computing and hybrid HPC-QC systems](https://enccs.github.io/NordIQuEst-workshop/)

Learning objectives:
- Learn key concepts: quantum states, qubits, quantum algorithms
- Get an overview of QC programming in high-level languages for use cases in optimisation, finance and quantum chemistry 
- Get an vverview of the main QC hardware approaches
- Understand how QC can be integrated with classical computing through hybrid classical/quantum algorithms and HPC-QC systems.
- Learn to perform quantum software testing with the Quito tool
