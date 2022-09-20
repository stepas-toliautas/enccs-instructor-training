# Lesson Development

```{questions}
- Are there any pedagogical best practices in developing lesson material?
- What tools and methods can be used to collaboratively develop training material?
```

```{objectives}
- Understand what is meant by backwards lesson design
```

## Backwards lesson design

When writing an ENCCS lesson, we take a “reverse” approach to instruction, 
as described in Wiggins and McTighe’s 
[Understanding by Design](http://www.worldcat.org/title/understanding-by-design/oclc/56491025),
that keeps the focus firmly on learning outcomes. The order of preparation in this case becomes

- Determine your learning objectives
- Decide what constitutes evidence that objectives have been met, and design assessments to target that evidence
- Design instruction: Sort assessments in order of increasing complexity, 
  and write content that connects everything together

### Deciding what to teach

![What to Teach](https://carpentries.github.io/instructor-training/fig/what-to-teach.png)


### Working with learning objectives

ENCCS lessons usually have a *learning objectives* section.
Good learning objectives are quite specific about the intended effect of a lesson on its learners.
We aim to create learning objectives that are specific, accurate, and informative for 
both learners and instructors.

In practice, it's best to start defining your target audience by answering to questions
such as:
- **What is the expected educational level of my audience?** 
- **Have they been already exposed to the technologies I am planning to teach?** 
- **What tools do they already use?** 
- **What are the main issues they are currently experiencing?**. 

Once you clarified your target audience, it is useful to create
**learner personas**. This will help you during the development process by
providing concrete examples of potential learners showing up at your
workshops. 

- For each **learner persona**, try to think of what is **useful to them**. 
- What do they **need** to remember/understand/apply/analyze/evaluate/create (see Bloom's taxonomy below).
- Then, you create a sequence of exercises which test incrementally
  progressing tasks and acquisition of the new skills.
- Finally, you write material to teach the gap between exercises.

### Using Bloom's Taxonomy to write effective learning objectives

[Bloom's Taxonomy](https://cft.vanderbilt.edu/guides-sub-pages/blooms-taxonomy/) is a framework for 
thinking about learning that breaks progress down into discrete, hierarchical steps.
While many ideas have come and gone in education, Bloom's has remained a useful tool for educators, 
in particular because the
hierarchy seems to be reasonably valid: outcomes at the top of the hierarchy cannot be achieved 
without mastery of outcomes at
the bottom. 

![Bloom's Taxonomy](https://carpentries.github.io/instructor-training/fig/Blooms.png)

Image credit: Vanderbilt University Center for Teaching

### Revisiting Learning objectives

When using existing teaching material, *backwards design*  principles might be applied as
follows:

1. Review the lesson's learning objectives carefully, thinking about how they will work for your audience
2. Scan the lesson to identify promising points to check in with your learners, using formative assessment to verify that objectives have been met
3. Review the connecting content in detail to be sure everything works and you have anticipated likely problems and questions.

We strongly encourage you to read Learning objectives before teaching a lesson and to review 
whether they still match the content of the lesson.

```{challenge} How do you design?
Discuss either in groups or via collaborative document:
- How do you start when you design a new lesson/presentation?
- Has your approach changed over the years? If yes, how?
```

---

## Designing exercises

Well designed examples and exercises can go a long way towards correcting misconceptions 
and expanding the mental models of learners.

The goal of exercises is twofold:
- instructors can assess the progress of learners.
- learners put in practice the skills that you have included in your skills list.

Here are some suggestions to keep in mind:

- Not every exercise has to be an amazing hand-on example. Mixing with smaller, more conceptual 
  things can reduce cognitive load.
- Try to make your exercises relevant, meaningful and connected to previous knowledge. 
  Connect the exercises to the real world. When learners understand the meaning of new concepts 
  it will be easier for them to remember.
- Create also more advanced exercises which can be optional for more advanced learners. This can go 
  a long way to meet the needs of participants with a wide range of background knowledge. 


Good exercises are the most important factor in a good lesson. Even if you are preparing the rest of 
the lesson mostly alone, consider a good long brainstorming session to go from "list of topics to 
cover" to "sequence of exercises".

When you are stuck thinking "how can I make an exercise that covers X", think of the lists below inspiration. Not every exercise has to be an sophisticated hands-on thing, so don’t be afraid to use different types:

Basic types:

- Multiple choice (easy to get feedback via a classroom tool - try to design each wrong answer so that it identifies a specific misconception).
- Code yourself (traditional programming)
- Code yourself + multiple choice to see what the answer is (allows you to get feedback)
- Inverted coding (given code, have to debug)
- Parsons problems (working solution but lines in random order, learner must only put in proper order)
- Fill in the blank

More advanced:

- Tracing execution
- Tracing values through code flow (e.g. what is the sequence of values that x takes on?)
- Reverse execution (find input that gives an output)
- Minimal fix (given broken code, make it work)
- Theme and variations (working code, adapt to other type of situation/problem)
- Refactoring

More conceptual:

- Draw a diagram
- Label diagram
- Matching problem: two sets of Q/A, match them.


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

```{challenge} Backwards-design a lesson
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
- Some aspect from an already existing lesson
- [An ENCCS lesson](https://enccs.se/lessons/) (or an episode therein)
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

Why static sites?
- Decentralized (in terms of organization/namespace)
- Forkable
- Anybody can suggest changes

- [Sphinx](https://www.sphinx-doc.org)-based
  - Example: this lesson
  - Starting point: [sphinx-lesson](https://github.com/coderefinery/sphinx-lesson)
  - [Documentation](https://coderefinery.github.io/sphinx-lesson/)
- Templates can be freely re-used


---

### Contributing to existing lessons

Our lessons are **collaboratively developed** and some are created by many
people. We encourage everyone to contribute to the lessons.

Lessons should be reviewed often - essentially, before each workshop by
the instructor of that workshop.  This can be a quick review, looking
at issues and fixing easy things, or more thorough.

Every so often, there is an extensive
hackathon period of fully revising a lesson and making major improvements.

CodeRefinery has a [lesson-review](https://coderefinery.github.io/manuals/lesson-review/) 
checklist to guide the review process.

```{discussion}
We now go to the
[lesson-review](https://coderefinery.github.io/manuals/lesson-review/)
checklist and discuss it, instead of duplicating things here.
```

---

### Collaborative workflows

There are two main ways to collaborate on lesson (or code) development 
on a repository-hosting website like [GitHub](https://github.com/), 
[GitLab](https://about.gitlab.com/) or [Bitbucket](https://bitbucket.org/).

**Centralized workflow**

![Centralized](https://coderefinery.github.io/git-collaborative/_images/centralized.svg)

- Typically all developers have both read and write permissions (double-headed arrows).
- Suited for cases where **all developers are in the same group or organization or project**.
- **Everybody who wants to contribute needs write access**.
- Good idea to write-protect the main branch (typically master or main).

**Forking workflow**

![Forking](https://coderefinery.github.io/git-collaborative/_images/forking-overview.svg)

In the **forking layout**, again we call one repository the “central” repository but people push to forks (their own copies of the repository on GitHub/GitLab/Bitbucket).

- **Anybody can contribute without asking for permission** (to public projects).
- Maintainer still has **full control over what is merged**.
- There is now **more than one remote** to work with.

`````{challenge} Practice collaborative workflow

Here we will practice the forking workflow. **NOTE**: You will need a 
[GitHub account](https://github.com/signup) to perform this exercise.

````{tabs}
```{tab} Centralised workflow

- The maintainer of the repository will first need to add you as contributors with write permissions.
- Navigate to [this example repository on GitHub](https://github.com/ENCCS/example-repository).
- Clone the repository to your computer by clicking the Code button
  and copy-paste the name of the remote. 
  Choose SSH if you have uploaded SSH keys to GitHub, otherwise go for HTTPS.
  Then go to a terminal on your computer, and type `git clone <copy-pasted-remote>`.  
  ![clone-button](img/clone-button.png)
- Best practice: create a new branch in your local repository: `git checkout -b <name/feature>` 
  (replace "name" with your name, and "feature" with a descriptor of your intended change).
- Now add a new plain-text file to the repository. You can create it with a terminal editor 
  (nano, emacs, vim) or a simple text editor. In the file, add either a famous quote, a cooking 
  recipe, a poem or something else that you like. 
- After the file is created, *stage* it with `git add <filename>`.
- After staging, *commit* the file with `git commit -m <some descriptive commit message>`.
- Now push your commit to your fork: `git push origin <name/feature>`
- In the output of the push command you will see a URL for creating a **pull request**. 
  Copy-paste it to a web browser. 
  ![git-push-output](img/git-push-output.png)  
  You can also just go to the page of the example repository - 
  there should be a new menu at the top inviting you to create a pull request.
  ![github-pr-menu](img/github-pr-menu.png)
- On the "Open a pull request" page, make sure that you are sending the pull request from 
  your feature branch to the main branch
  ![open-pr](img/open-pr.png)
- Finally, edit the title of the pull request and add a comment (optional), and then 
  click the green "Create pull request" button.
- You have now created a pull request and a collaborator can review your change, provide feedback 
  if needed (e.g. to ask for changes), and then merge it into the main branch!
```

```{tab} Forking workflow

- Navigate to [this example repository on GitHub](https://github.com/ENCCS/example-repository)
- Fork the repository to your own GitHub account by clicking the Fork button at the top.
  ![fork-button](img/fork-button.png)
  
- After the fork has been created, clone the repository to your computer by clicking the Code button
  and copy-paste the name of the remote. 
  Choose SSH if you have uploaded SSH keys to GitHub, otherwise go for HTTPS.
  Then go to a terminal on your computer, and type `git clone <copy-pasted-remote>`.  
  ![clone-button](img/clone-button.png)

- Best practice: create a new branch in your local repository: `git checkout -b <name/feature>` 
  (replace "name" with your name, and "feature" with a descriptor of your intended change).
- Now add a new plain-text file to the repository. You can create it with a terminal editor 
  (nano, emacs, vim) or a simple text editor. In the file, add either a famous quote, a cooking 
  recipe, a poem or something else that you like. 
- After the file is created, *stage* it with `git add <filename>`.
- After staging, *commit* the file with `git commit -m <some descriptive commit message>`.
- Now push your commit to your fork: `git push origin <name/feature>`
- In the output of the push command you will see a URL for creating a **pull request**. 
  Copy-paste it to a web browser. 
  ![git-push-output](img/git-push-output.png)  
  You can also just go to the page of your forked repository - 
  there should be a new menu at the top inviting you to create a pull request.
  ![github-pr-menu](img/github-pr-menu.png)
- On the "Open a pull request" page, make sure that you are sending the pull request from 
  your feature branch on your forked repository to the main branch of the parent repository
  ![open-pr](img/open-pr.png)
- Finally, edit the title of the pull request and add a comment (optional), and then 
  click the green "Create pull request" button.
- You have now created a pull request and a maintainer of the central repository 
  can review your change, provide feedback 
  if needed (e.g. to ask for changes), and then merge it into the main branch!

Bonus question: Why is it best practice to create a "feature" branch in your local repository?  
```
````
`````

```{callout} Why code review?
In collaborative software development, it is standard practice to review each other's 
code changes. This serves multiple purposes:
- Others in the team learn about your changes.
- An extra pair of eyes are useful to catch bugs or suggest improvements
- It's possible (and common) to enable *automated testing* so that each pull request is tested 
  automatically in the cloud so that the reviewer can see whether a pull request passes all 
  unit tests.

There's no reason not to apply these practices to collaborative lesson development!
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

```{keypoints}
- Having a semi-rigid lesson design process can **save time** to start drafting and will probably **increase quality and relevance** of the lessons 
```