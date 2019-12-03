# RL Winter Mentorship

This is the repository that contains all the material/code required to get
started with the mentorship programme. A few points of administration:

1. The length of the mentorship is around 5 weeks.

2. We assume you some prior knowledge of programming.

3. For an help with the course, you can privately contact your mentor. A better option
would be to [open an issue on this repository](https://help.github.com/en/github/managing-your-work-on-github/creating-an-issue),
so that others can see your
question, and it'll prevent any replicated effort on the part of the mentor.
All discussions related to code will happen over issues.

4. All your code will be pushed to GitHub, so if you haven't already, create
a GitHub account. Create a **private** repository with the name:
`rl-winter-mentorship` and add **only your mentor** as a collaborator. The
mentors GitHub IDs are: `@squadrick` (Dheeraj), `@sahas00` (Sahas).

5. Create a `README.md` in your repository where you can keep track of your
progress over the next month. The mentors will be using the `README.md` as
a progress tracker.

Don't be afraid to ask any questions (however irrelevant you think it may be).
The mentors are here to help you every step of the way.

For any issues with the GirlScript Winter Mentorship Programme please contact
Arpith or Akshatha.

## Prerequisites

  1. OS: Either some Linux based OS (Ubuntu, Fedora, etc.) OR Mac OSX. Windows
  will not suffice.

  2. Language: We'll be using Python3 throughout this course. So familiarise
  yourself with the language. Also learn to install packages using `pip`.

  3. Libraries:

      a. [NumPy](https://numpy.org/): Used for matrix computations.

      b. [OpenAI Gym](https://gym.openai.com/): Has a host of training
      environments with an easy-to-use API.

      c. [TensorFlow](https://www.tensorflow.org/) OR
      [PyTorch](https://pytorch.org/): Deep learning libraries that we'll use
      later on (week 4, 5) in the course to train neural networks. The choice is
      left entirely up to the mentee, but you can contact your mentor to narrow
      down the choice.

  4. Tools:

      a. Text Editor: You can use any editor of choice. Recommendations: VSCode,
      Atom, Vim, Emacs. You can also use an IDE if you wish, PyCharm is [free for
      students.](https://www.jetbrains.com/student/)

      b. `git`: You'll be using GitHub for all your code/assignment submission,
      so learn the basics of `git`: `pull`, `push`, `add`, `commit`.


## Scope

The scope of this course will be rather narrow due to the time constraint, but we
hope you'll learn the foundational level of reinforcement learning that'll
help you along the way when you decide to learn more advanced concepts.

1. Markov Decision Processes (MDPs): A formula mathematical framework for RL.

2. Tabular methods: Value iteration, policy iteration

3. RL with function approximators: Building and training a perceptron from
scratch to solve famous RL problems (CartPole, Mountain Car).

4. Imitation learning: You'll be competiting against your peers to see who
can perform the best in trying to imitate an expert to control a robot.

5. Intro to Deep RL: Brief introduction to using deep learning with RL to create
powerful general purpose solvers.

## Resources

Since every one prefers a different approach to learning, we're gonna try our
best to accomodate each style. Every topic has multiple levels of resources:

1. Intuitive: This will be a high level, *hand-wavy* explanation of the concepts.
This will not help you understand the core of the concept, but you will have a
general understanding.

2. Code: If you prefer to learn by looking at the codebase, we'll link open
source implementations of the algorithm (where appropriate).

3. Lectures: We'll link free online YouTube lectures.

4. TextBook: We'll link to chapters from this book -
[Sutton and Barto](https://web.stanford.edu/class/psych209/Readings/SuttonBartoIPRLBook2ndEd.pdf) (SnB).

The recommendation would be to either use Lectures or Text Books to get a
solid grasp of the conceptual details, and to use the Code as a reference
during the assignment. Please note that we don't tolerate any plagiarism.

At the end of each week you will be given a set of deliverables to complete.
This could either be a report, or a coding assignment. All submissions will
happen via GitHub.

## Detailed Breakdown

#### Week 0

Before the start of the course, we except you to have completed all the administration
work and prerequisites. Also, some *pop-sciency* knowledge never hurt anyone:

  1. [TextBook] Chaper 1 from SnB: The Reinforcement Learning Problem

  2. [Intuitive] [What is reinforcement learning?](https://deepsense.ai/what-is-reinforcement-learning-the-complete-guide/)

  3. [Lecture] [David Silver Lecture 1](https://www.youtube.com/watch?v=2pWv7GOvuf0)

  4. [Wikipedia article on RL](https://en.wikipedia.org/wiki/Reinforcement_learning)


#### Week 1

Mathematical foundation of RL - Markov Decision Processes.

  1. [TextBook] Chapter 3 from SnB: Finite Markov Decision Processes

  2. [Intuitive] [Reinforcement Learning Demystified: Markov Decision Processes](https://towardsdatascience.com/reinforcement-learning-demystified-markov-decision-processes-part-1-bf00dda41690)

  3. [Lecture] [David Silver Lecture 2](https://www.youtube.com/watch?v=lfHX2hHRMVQ)

Deliverables:

1. Solve Excercises 3.1, 3.2 and 3.3 from Sna (Page: 85). Write a report using
[Markdown](https://www.markdownguide.org/getting-started/) or Google Docs. Please
keep the answers as brief as possible, you won't be assessed on the length of
the report.

#### Week 2

Tabular methods

  1. [TextBook] Chapter 4 from SnB: Dynamic Programming

  2. [Intuitive, Code] [Medium article](https://medium.com/@m.alzantot/deep-reinforcement-learning-demysitifed-episode-2-policy-iteration-value-iteration-and-q-978f9e89ddaa)

  3. [Lecture] [David Silver Lecture 3](https://www.youtube.com/watch?v=Nd1-UUMVfz4)

Deliverables:

1. Solve all environments from [`gym-gridworlds`](https://github.com/podondra/gym-gridworlds)
using value and policy iteration using **only** NumPy.

#### Week 3

Function Approximators

  1. [TextBook] Chapter 9, 10, 11 from SnB
  2. [Lecture] David Silver: [Lecture 6](https://www.youtube.com/watch?v=UoPei5o4fps), [Lecture 7](https://www.youtube.com/watch?v=KHZVXao4qXs)
  3. [Code] [OpenAI Spinning Up](https://spinningup.openai.com/en/latest/)


Deliverables:

Build a single layer neural network using **only** NumPy to solve `CartPole` using:

  1. Q-Learning
  2. Vanilla Policy gradients


#### Week 4

Competition Week

We'll give you some data from an expert controlling a robot. Your task to create
the best agent either using the expert data or not. Throughout the week, we'll
maintain a leaderboard of scores, and each mentee can have multiple submissions.
The format for submissions will be announced later. (#TODO)

#### Week 5

Intro to Deep RL. The leap from the previous week to this will be quite substantial. 
The exact specifics of this week is open-ended, it's entirely up to the mentee
to decide what they want to pursue. A few potential options are:

  1. Reimplementing a seminal research paper like [DQN](https://www.cs.toronto.edu/~vmnih/docs/dqn.pdf), 
  [PPO](https://arxiv.org/abs/1707.06347), etc.
  
  2. Using [an existing library](https://github.com/openai/baselines) on new 
  unexplored environments like your favourite FPS game, or in more unconvential 
  problems like [solving symbolic integration](https://en.wikipedia.org/wiki/Symbolic_integration). 
  
You'll discuss with your mentor based on your progress to figure out what'll work 
best, focusing on your area of interest. 
