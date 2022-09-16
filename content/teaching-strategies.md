# How to teach online

```{objectives}
- Understand the benefits and disadvantage of online teaching,
  compared to in-person
- Set up a good screen share
- Understand the benefits and disadvantages of team teaching
- Prepare for the teaching practice
```

to add: 
- stick to the script (conflicting info inhibits learning)

## Why teaching mechanics matter

- When you teach, you are mainly showing a basic example for the
  learner to follow along
- The learner has a *lot* more to think about than you do, so you need
  to minimize the possible distractions and unnecessary weirdness.
- A learner will often only one small screen, limiting the number of
  things that they can think about.
- You are must faster than learners (5 times possibly?)  You have to
  do things to slow yourself down.
- It's easy to save these mechanics until the end, and then you run
  out of time.


### Shell sharing

```{discussion} Discussion: what goes into a good shell share or demonstration?

When you are following along with a type-along demonstration, what
things:

- Are useful to make it easy to follow along
- Make it harder to follow along

Answer in the collaborative notes
```

When doing any demonstration, there are difficulties:

- If one misses something, you can't rewind to see it - is there any
  way to catch up?
- The learner must get oriented with the whole picture, while
  instructor knows precisely where to focus.

A good **shell share** has some of the following properties:

- Large font
- Shell history, available separately from the main shell window
- Closely matches the type-along instructions

We have a collection of shell sharing systems:
- We will look over [lesson presentation
hints](https://coderefinery.github.io/manuals/instructor-tech-setup/#terminal-history-window).
- There are other things you can copy
- Whatever you do, do *something*.

```{discussion}
The instructor will demonstrate several shell-sharing systems.  You
will use this in the teaching practice.
```


### Screen sharing

`````{discussion}

Look at the various [screen layouts in the CodeRefinery
manuals](https://coderefinery.github.io/manuals/instructor-tech-setup/#screen-sharing).
Use the HackMD to comment about what which are better or worse.

````{output} HackMD prototype
:class: dropdown
```
- S1
  - good:
  - bad:
- S2
  - good:
  - bad:
- S3
  - good:
  - bad:
- S4
  - good:
  - bad:
- Student layouts:
  - ...
- Instructor layouts:
  - ...
```
````
`````

- Many learners will have a smaller screen than you.
- You should plan for learners with only one small screen.
- A learner will **need to focus on both your screen share and their
  work**.
- Sharing your a whole screen is almost always a bad idea, if you want
  the learners to do anything at the same time.
- If you constrict yourself, then your experience is more similar to
  that of a learner.

Vertical sharing:
- CodeRefinery has recently started trialing a **vertical share**
  system, where you share a vertical half of your screen.
- This allows learners with one screen to display your screen
  side-by-side with their learn
- Zoom provides a "Share a part of screen" that is good for this.



### Meta-talk

Don't just teach, also make sure you guide the learners through the
course.

- You know what you just discussed, and what is coming next, but
  learners are often stuck thinking about now.
- Give a lot of "meta-talk" that is not just about the topic you are
  teaching, but how you are teaching it.
- Examples
  - **Why** you are doing each episode
  - What is the purpose of each exercise
  - Clearly state what someone should accomplish in each exercise and
    how long it will take - don't assume this is obvious.
  - What is the point of each lesson.  How much should people expect
    to get from it?  Should you follow everything, or are some things
    advanced and optional?  Make that clear.

## The importance of going slow

It takes work to actively assess mental models throughout a workshop; this also takes time. This can make Instructors feel conflicted about using formative assessment routinely. However, the need to conduct routine assessment is not the only reason why a workshop should proceed more slowly than you think.

Because your learners’ mental models will likely be less densely connected than your own, a 
conclusion that seems obvious to you will not seem that way to your learners. It is important to 
explain what you are doing step-by-step, and how each step leads to the next one.

Experts are also better at diagnosing errors than novices or competent practitioners. If faced with an error message while teaching, an expert will often automatically diagnose and solve a problem before a novice has even finished reading the error message. Because of this, it is very important while teaching to be explicit about the process you are using to engage with errors, even if they seem trivial to you, as they often will.


## Team teaching

Demonstration-based teaching require two different types of focus:
- Doing the mechanical steps as a demonstration
- Explaining why you are doing it

This is a lot for one person to keep in mind, so can multiple people
work together for this? Team teaching idea:
- One person is doing the demonstrations
- One person is giving the commentary about what they are doing
- The lecture becomes a discussion between two people instead.

```{callout} Co-teaching

   Wikipedia: Co-teaching or team teaching is the division of labor
   between educators to plan, organize, instruct and make assessments
   on the same group of students, generally in the a common
   classroom,[1] and often with a strong focus on those teaching as a
   team complementing one another's particular skills or other
   strengths.
```

Advantages:
- The course seems very interactive, much more so than expecting
  students to speak up.  The co-teacher can take on the "voice of the
  audience".
- Quicker preparation time since co-teachers can rely on each other in
  unexpected situations.
- One co-teacher can be effectively learning at the same time and thus
  acting as the "voice of the audience" in another way.
- Great way to onboard new instructors - extensive training and
  preparation no longer needed.
- More active minds means better able to watch and react to other
  feedback, such as HackMD or chat.
- Less workload - one person does not have to prepare perfectly, any
  uncertainty can usually be quickly answered by the other.


Disadvantage:
- Requires two people's time
- Requires coordination when preparing (slows you down in preparation)
- Unfamiliar concept to most people

### Strategies

In reality, these strategies are mixed and matched even within a
lesson, and there are many things between these:

- One person gives lectures, one does the typing during demos.
- "Interview": One primarily doing the "teaching", one guiding by
  asking questions - either as an interviewer or as a virtual learner.

Things that don't work (are not team teaching):

- Dividing up a lesson into parts, each person gives different parts
  independently.

---

## Questions

- Questions are great, and important for any practical and interactive
  class
- But questions in main room doesn't scale to very large rooms.
- ENCCS strategy: HackMD for questions
  - Chat is not good enough, you can't reply to old things
  - HackMD allows threaded replies and follow up later
  - You need some other helpers to watch HackMD and answer, and bring
    things up to you.  And let you know how things are going.
  - Learners can ask anonymously
  - Learners don't have to worry about interrupting the flow.
  - Disadvantage: can produce information overload, warn people to not
    follow too closely
  - With too few people, it can turn out to be very quiet.


## Keeping learners motivated

**Invite Participation**

- Having, discussing, and enforcing a Code of Conduct provides a framework for positive 
  communication to occur.
- Encourage learners to learn from each other. Working in pairs or in groups encourages learners to 
  talk through their learning process, reinforcing memory and making it more likely that confusion 
  will be expressed and resolved. This can also address challenges of varying background experience: 
  asking more advanced learners to help beginners can maximize learning for both. In these cases, 
  make sure the beginner is doing the typing!
- Acknowledging when learners are confused. Acknowledging and exploring confusion with kindness 
  rewards learners for sharing vulnerable information. Formative assessments can pinpoint misunderstandings. When learners see that 
  others are confused, they are more likely to share their own uncertainties.



**Do no harm!**  
Here are a few things you should not do in your workshop:

- Talk contemptuously or with scorn about any tool or practice, or the people who use them. 
  Regardless of its shortcomings, many of your learners may be using that tool, and may have invested many years in learning to do so. 
- Dive into complex or detailed technical discussion with the one or two people in the audience who 
  clearly don't actually need to be there. Reserve those conversations for breaks or follow-up emails.
- Pretend to know more than you do. People will actually trust you more if you are frank about the 
  limitations of your knowledge, and will be more likely to ask questions and seek help. 
- Use the J word ("just") or other demotivating words. Experts sometimes want to convey that 
  a task is as easy as they think it is, but these signal to the learner that the instructor thinks 
  their problem is trivial
- Take over the learner's keyboard. It is rarely a good idea to type anything for your learners. 
  Doing so can be demotivating for the learner (as it implies you don't think they can do it themselves or that you don't want to wait for them). It also wastes a valuable opportunity for your learner to develop muscle memory and other skills that are essential for independent work.
- Express surprise at unawareness. Saying things like "I can’t believe you don’t know X" or "You’ve 
  never heard of Y?" signals to the learner that they do not have some required pre-knowledge of the 
  material you are teaching, that they don’t belong at the workshop, and it may prevent them from 
  asking questions in the future.

**Does your motivation matter?**

- Learners respond to an instructor’s enthusiasm. The more motivated you are, the more motivated 
  they will be!
- Instructors are learning to teach. This also takes motivation. Deliberative practice, seeking 
  feedback, and reflecting on mistakes in the context of your own busy work life is a challenge. 
  What will keep you energized to stay engaged with your learning process?

## See also

- [Instructor tech setup](https://coderefinery.github.io/manuals/instructor-tech-setup/)
- [Lesson preparation hints](https://coderefinery.github.io/manuals/presenting/) (more focused on in-person)
- [Instructor introduction](https://coderefinery.github.io/manuals/presenting/) -
  has a lot of tips for new instructors, but also more things about
  the workshop.
- [HackMD mechanics](https://coderefinery.github.io/manuals/hackmd-mechanics/) and [HackMD helpers](https://coderefinery.github.io/manuals/hackmd-helper/).  
- [Workshop prep call](https://coderefinery.github.io/manuals/workshop-prep-call/)
- [Team teaching](https://coderefinery.github.io/manuals/team-teaching/)

