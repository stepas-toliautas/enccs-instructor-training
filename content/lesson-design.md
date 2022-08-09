# Lesson design

```{questions}
- Are there any pedagogical best practices in developing lesson material?
- What tools and methods can be used to collaboratively develop public lessons?
```

## Backwards lesson design

When writing an ENCCS lesson, we take a “reverse” approach to instruction, 
as described in Wiggins and McTighe’s 
[Understanding by Design](http://www.worldcat.org/title/understanding-by-design/oclc/56491025),
that keeps the focus firmly on learning outcomes. The order of preparation in this case becomes

- Determine your learning objectives
- Decide what constitutes evidence that objectives have been met, and design assessments 
  to target that evidence
- Design instruction: Sort assessments in order of increasing complexity, 
  and write content that connects everything together

### Working with learning objectives

Each ENCCS lesson (also the HPC capentries lessons) usually has a *learning objectives* section.
Good learning objectives are quite specific about the intended effect of a lesson on its learners.
We aim to create learning objectives that are specific, accurate, and informative for 
both learners and instructors.


### Using Bloom's Taxonomy to write effective learning objectives

[Bloom's Taxonomy](https://cft.vanderbilt.edu/guides-sub-pages/blooms-taxonomy/) is a framework for thinking about learning that breaks progress down into discrete, hierarchical steps.
While many ideas have come and gone in education, Bloom's has remained a useful tool for educators, in particular because the
hierarchy seems to be reasonably valid: outcomes at the top of the hierarchy cannot be achieved without mastery of outcomes at
the bottom. In the long term, everybody wants to be at the top. However, in aiming to meet learners where they are, we also
need to be mindful about helping them to ["grow a level,"](https://software-carpentry.org/blog/2018/03/tractenberg-summary.html) helping them to recognize when they have achieved that growth, and
guiding them to look ahead to where we might not be able to take them.

![Bloom's Taxonomy](https://carpentries.github.io/instructor-training/fig/Blooms.png)

Image credit: Vanderbilt University Center for Teaching

### Revisiting Learning objectives

When using existing teaching material, *reverse instructional design*  principles might be applied as
follows:

1. Review the lesson's learning objectives carefully, thinking about how they will work for your audience
2. Scan the lesson to identify promising points to check in with your learners, using formative assessment to verify that objectives have been met
3. Review the connecting content in detail to be sure everything works and you have anticipated likely problems and questions.


We strongly encourage you to read them before teaching a lesson and to review whether they still match the content of the lesson: 


## How do you design?

```{discussion}
Discuss either in groups or via collaborative document:
- How do you start when you design a new lesson/presentation?
- Has your approach changed over the years? If yes, how?
```

---

## Backwards lesson design

### The approach

- You don't think about how to do something and try to explain it.
- Avoid the typical approach *"I want to show a number of things which I think are cool about
  tool X - how do I press these into 90 minutes?"*
- Instead, you start defining your target audience by answering to questions
  such **What is the expected educational level of my audience?**, **Have they
  been already exposed to the technologies I am planning to teach?**, **What
  tools do they already use?**, **What are the main issues they are currently
  experiencing?**. It is important to discuss these points with a group of
  colleagues, preferably from diverse backgrounds and institutions to reduce
  biases. Once you clarified your target audience, it is useful to create
  **learner personas**; that will help you during the development process by
  providing concrete examples of potential learners showing up at your
  workshops. For each **learner personas**, try to think of what is **useful to
  them**: *"What do they **need** to
  [remember/understand/apply/analyze/evaluate/create](https://coderefinery.github.io/instructor-training/03-teaching-style/#using-bloom-s-taxonomy-to-write-effective-learning-objectives)?"*.
  Asking and answering to these questions will allow you to define the
  background knowledge (starting points) and goals (end points) of your
  learners.  Then, you create a sequence of exercises which test incrementally
  progressing tasks and acquisition of the new skills (from starting to end
  points).
- Then, you write the minimum amount
  of material to teach the gap between exercises.

### The process

For the whole process, see [our
manual](https://coderefinery.github.io/manuals/lesson-design/#backwards-lesson-design)
(instructor discusses these points briefly).


### Why is it good to have a process?:

- Having a semi-rigid design process can **save time** to start drafting.
- It allows collaborative development of teaching material.
- It will probably **increase quality and relevance** of lessons for learners.
- **We aren't perfect yet.**  CodeRefinery is still striving to get
  better at this, and we are more ad-hoc than you might think.
  A number of our lessons have not been designed this way but we are now improving
  these lessons with the backwards lesson design in mind.


### Designing exercises


The goal of exercises is twofold:
- instructors can assess the progress of learners.
- learners put in practice the skills that you have included in your skills list.

When designing exercises, consider that some participants will get stuck
and may want to re-join at a later exercise. In other words it is nice
if exercises build up on each other but not at the cost that if participants
get stuck at exercise 2, they will not be able to do exercises 3 to N.

---

## Practice backwards design


```{discussion} The goal here is to discuss and provide examples on backwards-design of a lesson.

Let's take as an example the *[HPC Carpentry lesson](https://hpc-carpentry.github.io/hpc-intro/)*

**Target audience**
  - What is the expected educational level of my audience?
      - A PhD student, postdoc or young researcher.
  - Have they been already exposed to the technologies I am planning to teach?
      - The word **HPC** is not new to them and they may have already used an HPC but are still not capable of giving a proper definition of HPC. In addition, we do not expect them to know much about parallelism and they cannot make any distinction between various available parallelism paradigms.
  - What tools do they already use?
      - serial codes, multi-threaded codes, data parallelism; usually out-of-the-box tools.
      - they may have tried to "scale" their code (multiprocessing, threading, GPUs) with more or less success.
  - What are the main issues they are currently experiencing?
      - they cannot solve their problems either because they would like to run the same code but with many different datasets or because their problem is larger (more computations/memory).
      - most of the time they know their codes can run on HPC (from the documentation) but never really had the opportunity to try it out.
      - Very few will have their own codes where they may have tried different things to speed it up (threading, task parallelism) but have no clear strategy.

**Learner persona**
  - Sonya is a 1st year PhD student: she recently moved to Oslo and joined the
    Computational and Systems Neuroscience group. She will be using the
    [NEST](https://nest-simulator.readthedocs.io/), a simulator for spiking
    neural network model. She used NEST during her master thesis but on her
    small cluster: **she never used an HPC resource** and is really excited about it.
  - Robert is a field ecologist who obtained his PhD 6 months ago. He is now
    working on a new project with Climate scientists and as a consequence will
    need to run global climate models. He is **not very familiar with command
    line** even though he attended a Software Carpentry workshop and the idea to
    use HPC is a bit terrifying. He knows that he will get support from his
    team who has extensive experience with HPC but would like to become more
    independent and be able to **run his own simulations** (rather than copying
    existing cases).
  - Jessica is a postdoc working on a project that investigates numerically the
    complex dynamics arising at the tip of a fluid-driven rupture. Fluid
    dynamics will be computed by a finite element method solving the
    compressible Navier-Stokes equations on a moving mesh. She **uses a code she
    has developed** during her PhD and that is based on existing libraries. She
    has mostly ran it on a local desktop; her work during her PhD was very
    limited due to the lack of computing resources and she is now very keen is
    **moving to HPC**; she knows that it will requires some work, in particular to
    parallelize her code. This HPC training will be her first experience with
    HPC.

**Learning outcomes**
  - Understand the difference between HPCs and other local/remote machines
  - Understand the notion of core, nodes, cluster, shared/distributed memory, etc.
  - Understand the notion of login nodes.
  - Understand the need for a scheduler and how to use it appropriately
  - Understand why optimising I/O is important on HPC and how to best use HPC filesystems
  - Understand the need to parallelize (or use existing parallel) codes and in which cases HPCs is a must (when communications is required)
  - Understand how to get your code ready to use on HPC (access to libraries, installation of your own libraries/software, etc.)
  - Understand that an HPC is an operational machine and is not meant for developing codes.

**Exercises**
  - Get basic information such the number of CPUs, memory from your laptop and try to do the same on a HPC. Discuss outcomes.
  - Try to create files on the different filesystems on your HPC resource and access them.
  - Create different types of job scripts, submit and check outputs.
  - Make a concrete example to run a specific software on your HPC (something like GROMACS).
```

```{challenge} Demo
Before we let participants present to their groups, one of the instructors
presents a 5-minute segment and we practice together giving feedback.

The section we demo should require screen sharing and be of some follow-along
task.

If there is time, we present one demo on the day before, and one demo just
before the group exercise.
```

```{challenge} Exercise
Choose a simple lesson topic and apply backwards lesson design.  You
won't get all the way through, but come up with a logical
progression of exercises.

The section you pick should require **screen sharing** and be of some **follow-along
task** (preferably using a shell).

Some suggestions:
- Regular expressions
- Making papers in LaTeX
- Making figures in your favorite programming language
- Linux shell basics
- Something non-technical, such as painting a room
- An instructor training for CodeRefinery
- Some aspect from an already existing lesson
- [Introduction to high-performance computing](https://hpc-carpentry.github.io/hpc-intro/) (or an episode therein)
- [Unix shell in a HPC context](https://hpc-carpentry.github.io/hpc-shell/) (or an episode therein)
- A lesson you always wanted to teach

Exercise (30 minutes):
- Collect notes in a shared document.
- Start with learner personas and learning outcomes.
- Come up with a logical progression of exercises.

Discussion (15 minutes):
- How does this approach compare to other lessons or courses you have designed?
- We read, compare, and discuss our notes.
```

## Collaborative lesson development

This session focuses on **organizational** and **technical aspects**
of collaborative lesson development.

```{discussion}
This session is about **collaborative** lesson development. What advantages do
you see in developing lessons collaboratively and sharing lessons (making
material accessible)?  What difficulties are there?
```

---

### Lesson templates for static sites

- [Jekyll](https://jekyllrb.com/)-based
  - Example: [Introduction to version control with Git](https://coderefinery.github.io/git-intro/)
  - [Lesson template](https://github.com/coderefinery/example-lesson)
  - Common styling implemented as Git submodule: [jekyll-common](https://github.com/coderefinery/jekyll-common)
  - Based on a past version of the [Carpentries lesson style](https://github.com/carpentries/styles/)
  - A new Carpentries lesson template is in the works
- [Sphinx](https://www.sphinx-doc.org)-based
  - Example: this lesson
  - Starting point: [sphinx-lesson](https://github.com/coderefinery/sphinx-lesson)
  - [Documentation](https://coderefinery.github.io/sphinx-lesson/)
- Templates can be freely re-used

Why static sites?
- Decentralized (in terms of organization/namespace)
- Forkable
- Anybody can suggest changes

---

### Creating new teaching material

Creating new teaching material is a longer process, because you should
go through the whole
[backwards lesson design process](/lesson-design/)
and get extensive comments.
Still, don't feel afraid: nothing is perfect (or even good)
the first time. In fact, **it may be an advantage to share an imperfect
lesson with others early** to collect feedback and suggestions before the lesson
"solidifies" too much. Draft it and collect feedback. The result will probably
be better than working in isolation towards a "perfect" lesson.

```{discussion}
How can we share unfinished work/ideas?
- Draft pull requests (GitHub) or WIP (work in progress) merge requests (GitLab).
- Open an issue and discuss your idea before implementing it.
```

---

### Contributing to existing lessons

Our lessons are **collaboratively developed**.  They are made by many
people, and there is no single fixed master plan (but there should be,
in the instructors or maintainer's guide).  We encourage
everyone to contribute to the lessons.

Lessons are reviewed very often - essentially, before each workshop by
the instructor of that workshop.  This can be a quick review, looking
at issues and fixing easy things, or more thorough.

Every so often (such as at this training), there is an extensive
hackathon period of fully revising a lesson and making major improvements.

We've made the [lesson-review](https://coderefinery.github.io/manuals/lesson-review/) checklist
to guide the review process.

```{discussion}
We now go to the
[lesson-review](https://coderefinery.github.io/manuals/lesson-review/)
checklist and discuss it, instead of duplicating things here.
```

---

## Recommendations and lessons learned

- Convert feedback about lessons and suggestions for improvements into *issues*
  so that these don't get lost.
- Make your lesson citable: get a DOI.
- Credit contributors (not only Git commits).
- Instructor guide is essential for new instructors.
- Lesson changes should be accompanied with instructor guide changes (it's like
  a documentation for the lesson material).
- Apply and validate backwards lesson design again and again.
- Make it possible to try out new ideas (by making the lesson branch-able).
- Before making larger changes, talk with somebody and discuss these changes.
- For substantial changes we recommend to first open an issue and describe your
  idea and collect feedback before you start with an extensive rewrite.
- For things still under construction, open a draft pull request to collect
  feedback and to signal to others what you are working on.


## See also

- CodeRefinery [lesson-design](https://coderefinery.github.io/manuals/lesson-design/) manual
- [The Carpentries Curriculum Development Handbook](https://cdh.carpentries.org)
- [Teaching Tech Together](http://teachtogether.tech/)
- Our [summary](https://coderefinery.github.io/manuals/teaching-tech-together/) of "Teaching Tech Together"
- [Ten quick tips for creating an effective lesson](https://doi.org/10.1371/journal.pcbi.1006915)
