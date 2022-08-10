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
{: .discussion}

> ## About The Carpentries
> 
> [The Carpentries](https://carpentries.org/) is an international project that comprises [Software Carpentry](https://software-carpentry.org/) and [Data Carpentry](https://datacarpentry.org/), 
> communities of instructors, trainers, maintainers, helpers, and supporters who share a mission to 
> teach foundational computational and data science skills to researchers. The Carpentries teach 
> foundational coding and data science skills to researchers worldwide.
{: .discussion}


---

## Target audience

### Carpentries audience


The Carpentries aims to teach computational **competence** to learners through an applied approach, avoiding the theoretical and general in favor of the practical and specific.
**Learners do not need to have any prior experience in programming.**  One major goal of a Carpentry workshop is to raise awareness on the tools researchers can learn/use to speed up their research.

By showing learners how to solve specific problems with specific tools and providing hands-on practice, learners develops confidence for future learning.

> ## Novices
> We often qualify Carpentry learners as **novices**: they do not know what they need to learn yet. A typical example is the usage of version control: the Carpentry `git` lesson aims to give a very high level conceptual overview of Git but it does not explain how it can be used in research projects.
{: .callout}


### CodeRefinery audience

CodeRefinery workshops differ from Carpentry workshops as the audience is assumed to already write code and scripts and we aim at teaching them **best software practices**.

CodeRefinery learners usually do not have a good overview of **best software practices** but are aware of the need to learn them. Very often, they know the tools (Git, Jupyter, etc.) we are teaching but have difficulties to make the best use of them in their software development workflow.

> ## Competent practitioners
> We often qualify CodeRefinery learners as **competent practitioners** because they already have an understanding of their needs.
> *Novices* and *competent practitioners* will be more clearly defined in the {doc}`next section <teaching-style>`.
{: .callout}


### ENCCS audience

Similarly to CodeRefinery, ENCCS targets **competent practitioners**: participants are assumed 
to know what their needs are. Typically, their needs are to learn a technique or method to adapt 
their code to HPC, to learn novel programming languages or frameworks, or to deepen their knowledge 
of machine learning methods.

> ## Best software practices
> We cannot assume that ENCCS workshop participants are aware of best software development 
> practices. It is therefore wise to adhere to good practices when teaching ENCCS workshops 
> (e.g. by using version control and testing in code examples), so that participants  
> become acquainted with such practices.
{: .callout}


---


```{discussion} What we do differently?
- Planning, teaching material available in advance and not PDF slides
- Interactive, hands-on teaching. Presentations interleaved with exercises
- Different teaching roles (instructor, host, hackmd, ...)
- Helper recruitment 
- Less is more
- Clearly defining learning outcomes
- Asking for feedback, encouraging feedback
- Clearly defined code of conduct
- Screen-sharing
- Using lesson templates
- Lesson review on GitHub
- Sharing material open source instead of being protective
```

```{challenge} Ice-breaker in groups (10 minutes)
- Share your approach to teaching and your teaching philosophy with your group.
- Please share your tricks and solutions in the live document for others.
Additional ice-breaker questions:
- What is your motivation for taking this training?
- How structured or informal are your own teaching needs?
- What difference do you notice between the teaching what we (also
  CodeRefinery/Carpentries) do and traditional academic teaching?
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
