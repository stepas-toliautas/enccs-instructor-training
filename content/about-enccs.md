```{instructor-note}
   - 15 min teaching
```   

# About ENCCS

ENCCS (EuroCC National Competence Center Sweden) is one of 33 
nodes of the [EuroCC project](https://www.eurocc-access.eu/), which is funded by the 
European High-Performance Computing Joint Undertaking (EuroHPC-JU). As an NCC, we act as the central point of contact for HPC and related technologies in Sweden.
Our mission is to empower Swedish industry, academia and the public sector to leverage HPC, AI, and HPDA efficiently and effectively. 

Training is one of the main pillars of ENCCS' activities. We have developed a large amount of 
public and open source [lesson material](https://enccs.se/lessons/) and have taught over 45 
online workshops since September 2020. 
Our training philosophy and methods are to a large extent derived from two well established 
educational initiatives: [CodeRefinery](https://coderefinery.org/) and [The Carpentries](https://carpentries.org/). The material presented here covers both pedagogical ideas and practical 
aspects which underpin the development of lesson material, organisation of online or in-person 
workshops and the teaching itself.




---

> ## About CodeRefinery
>
> [CodeRefinery](https://coderefinery.org/) is a [Nordic e-Infrastructure Collaboration (NeIC)](https://neic.no/) project that started in October 2016.
> The main goals of CodeRefinery are:
> - Develop and maintain training material on software best practices for researchers that already write code. Our material addresses all academic disciplines and tries to be as programming language-independent as possible.
> - Provide a [code repository hosting service](https://coderefinery.org/repository/) that is open and free for all researchers based in universities and research institutes from Nordic countries.
> - Provide training opportunities in the Nordics using Carpentries and CodeRefinery training materials.
> - Articulate and implement the CodeRefinery sustainability plan.
{: .callout}

> ## About The Carpentries
> 
> [The Carpentries](https://carpentries.org/) is an international project that comprises [Software Carpentry](https://software-carpentry.org/) and [Data Carpentry](https://datacarpentry.org/), 
> communities of instructors, trainers, maintainers, helpers, and supporters who share a mission to 
> teach foundational computational and data science skills to researchers. The Carpentries teach 
> foundational coding and data science skills to researchers worldwide.
{: .callout}


---

## Target audience

### Carpentries audience


The Carpentries aims to teach computational **competence** to learners through an applied approach, avoiding the theoretical and general in favor of the practical and specific.
**Learners do not need to have any prior experience in programming.**  One major goal of a Carpentry workshop is to raise awareness on the tools researchers can learn/use to speed up their research.

By showing learners how to solve specific problems with specific tools and providing hands-on practice, learners develops confidence for future learning.

> ## Novices
> Carpentry learners can be qualified as **novices**: they do not know what they need to learn yet. A typical example is the usage of version control: the Carpentry `git` lesson aims to give a very high level conceptual overview of Git but it does not explain how it can be used in research projects.
{: .callout}


### CodeRefinery audience

CodeRefinery workshops differ from Carpentry workshops as the audience is assumed to already write code and scripts and we aim at teaching them **best software practices**.

CodeRefinery learners usually do not have a good overview of **best software practices** but are aware of the need to learn them. Very often, they know the tools (Git, Jupyter, etc.) we are teaching but have difficulties to make the best use of them in their software development workflow.

> ## Competent practitioners
> CodeRefinery learners can be qualified as **competent practitioners** because they already have an understanding of their needs.
> *Novices* and *competent practitioners* will be more clearly defined in the {doc}`next section <teaching-style>`.
{: .callout}


### ENCCS audience

Similarly to CodeRefinery, ENCCS targets **competent practitioners**: participants are assumed 
to know what their needs are. Typically, their needs are to learn a technique or method to adapt 
their code to HPC, to learn novel programming languages or frameworks, or to deepen their knowledge 
of machine learning methods.

> ## Best software practices
> We cannot assume that ENCCS workshop participants are aware of best software development 
> practices. It is therefore recommended to adhere to good software development practices when teaching ENCCS workshops 
> (e.g. by using version control and testing in code examples), so that participants  
> become acquainted with them as a side benefit of attending a workshop.
{: .callout}


---


```{discussion} What we do differently?
- Teaching material available in advance and not PDF slides
- Interactive, hands-on teaching. Presentations interleaved with exercises
- Different teaching roles (instructor, host, hackmd, ...)
- Helper recruitment 
- Less is more
- Clearly defining learning objectives
- Asking for feedback, encouraging feedback
- Clearly defined code of conduct
- Thoughtful screen-sharing
- Using lesson templates
- Lesson review on GitHub
- Sharing material open source instead of being protective.
```

```{challenge} Ice-breaker in groups (10 minutes)
- Share your approach to teaching and your teaching philosophy with your group.
- Please share your tricks and solutions in the live document for others.

Additional ice-breaker questions:
- What is your motivation for taking this training?
- How structured or informal are your own teaching needs?
- What other skills need to be taught, but academic teaching isn't the right setting?
```

````{challenge} What are the top issues new instructors face? (10 minutes)

Brainstorm about what issues new teachers/instructors might face in interactive workshops.
Write down your thoughts in the shared document.
 
```{solution} Some suggestions
 -  Breaks are not negotiable, minimum 10 minutes per hour.
 -  Exercise sessions too short. Better to have them as long as possible.
 -  Get the speed correct. Not too fast and not too slow. 
 -  Cater to participants with different backgrounds and at different levels of experience
 -  People will accomplish less than you expect. Expect learners to be 5 times slower than you, at best!
 -  Installation instructions not sufficiently complete. Installation will go wrong for some participants.
 -  Trying to accomplish too much or go through everything: it's OK to cut out and adapt to the audience. 
    Have a reserve session at the end that you prepare, but are ready to skip.
 -  Explaining *how*, but not *why*.
 -  Not making your environment match the learner's.
 -  Not setting up good screen sharing practices (terminal history, portion of screen).
 -  Assuming learners remember what they have already learned, or know the prerequisites. Or have stuff installed and configured.
 -  Not managing expectations: learners think that you will accomplish everything, and feel sad when you don't.
 -  Special issues when lessons delivered online (discussed during "How to teach online")
```
````

## ENCCS lessons

Below is a list of current ENCCS lessons along with their intended learning outcomes. 
These lessons are at different maturity levels and have been developed by many different people, 
so they do not all conform equally well to the recommendations presented in this lesson!


### GPU computing

#### [OpenMP for GPU Offloading](https://enccs.github.io/openmp-gpu/miniapp/)

- Get an overview of the architecture of GPU and how they differ from CPUs
- Understand how OpenMP fits into the landscape of GPU programming approaches
- Understand OpenMP's shared parallel model and program execution model
- Learn how to use basic OpenMP directives and clauses

#### [OpenACC](https://enccs.github.io/OpenACC/)

- Get an overview of the architecture of GPU and how they differ from CPUs
- Understand how OpenACC fits into the landscape of GPU programming approaches
- Understand OpenACC's shared parallel model and program execution model
- Learn how to use basic OpenACC directives and clauses

#### [Intermediate CUDA](https://enccs.github.io/CUDA/)

- Get an overview of the architecture of GPU and how they differ from CPUs
- Understand GPU concepts like threads, blocks and streaming multiprocessors 
- Learn to write simple CUDA kernels
- Learn to work with GPU memory
- Learn to optimize CUDA kernels
- Understand asynchronous execution

#### [SYCL](https://enccs.github.io/sycl-workshop/)

- What is SYCL and why it is useful.
- Write hardware-agnostic code to express parallelism using the queue, command group, and kernel abstractions.
- Use buffer and accessors to handle memory across devices.
- Evaluate drawbacks and advantages of unified shared memory.
- Get acquainted with the SYCL profiling API.

### HPC

#### [Intermediate MPI](https://enccs.github.io/intermediate-mpi/)

- Understand communicators, groups and derived datatypes
- Learn to use one-sided communication
- Understand and be able to use collective communication, blocking and non-blocking
- Understand how to work with MPI and threads

### Programming languages

#### [High-performance Data Analytics with Python](https://enccs.github.io/HPDA-Python/)

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

#### [Julia for High Performance Scientific Computing](https://enccs.github.io/Julia-for-HPC/)

- Experienced practioners in other languages understand what's different/special about Julia
- Become familiar with typical structure of a Julia package
- Set up efficient workflow for developing in Julia and using the package manager
- Learn to efficiently work with data 
- Know what performance pitfalls exist and learn to benchmark and profile code
- Learn to use multithreading and distributed computing
- Understand what different approaches exist for porting code to GPUs

### AI

#### [Upscaling A.I. training](https://enccs.github.io/upscalingAItraining/)

- Learn different strategies to perform distributed training in TensorFlow
- Learn how to use Horovod for distributed training
- Learn to containerise neural network training

#### [A.I. as a Tool for Change](https://www.youtube.com/watch?v=_FMnopQNF3M)

- Get an overview of possible use cases for artificial intelligence
- Understand how AI can effectively be put to use in different sectors and application domains
 

#### [Graph Neural Networks and Transformer](https://enccs.github.io/gnn_transformers/)

- Learn to use graph neural networks
- Learn to use transformers

### Applications

#### [Gromacs GPU Performance](https://enccs.github.io/gromacs-gpu-performance/)

- Understand the difference between MPI ranks and OpenMP threads when running GROMACS
- Be able to name the most important parts of the molecular dynamics workflow
- Appreciate some of the internal architecture of mdrun
- Know how to assign the PME workload
- Know how to use several GPUs efficiently.
- Know common pitfalls to avoid


#### [VeloxChem: Quantum chemistry from laptop to HPC](https://enccs.github.io/veloxchem-workshop/)

- Learn to perform quantum chemical simulations of ground- and excited-state properties of large systems using VeloxChem.
- Leverage the aggregate resources of modern HPC clusters to efficiently tackle large molecular systems.
- Use the Python application programming interface (API) to prototype new methods.
- Design interactive computational teaching materials in Python.

 
#### [OpenFOAM](https://enccs.github.io/OpenFOAM/)

- Learn how to use OpenFOAM



### Other

#### [CMake](https://enccs.github.io/cmake-workshop/)

- Write a CMake build system for C, C++, and Fortran projects producing libraries and/or executables.
- Run tests for your code with CTest.
- Ensure your build system will work on different platforms.
- Detect and use external dependencies in your project.
- Safely and effectively build mixed-language projects (Python+C/C++, Python+Fortran, Fortran+C/C++)

#### [Containers](https://enccs.github.io/Containers/)

- Learn to use Docker
- Learn to use Singularity

#### [Introduction to Quantum Computing and hybrid HPC-QC systems](https://enccs.github.io/NordIQuEst-workshop/)

- Learn key concepts: quantum states, qubits, quantum algorithms
- Get an overview of QC programming in high-level languages for use cases in optimisation, finance and quantum chemistry 
- Get an vverview of the main QC hardware approaches
- Understand how QC can be integrated with classical computing through hybrid classical/quantum algorithms and HPC-QC systems.
- Learn to perform quantum software testing with the Quito tool
