# AEM 7130 Dynamic Optimization
**Time**: Monday and Wednesday 11:25-12:40

**Location**: Statler 453
**abcdef**
**Office Hours**: Tuesday 3-4

**Prerequisites**: ECON 6090 and ECON 6170

**Credit Hours**: 3

**Programs**: You will need to install the following programs on your computer

- [Git](https://git-scm.com/downloads)
- [Julia](https://julialang.org/downloads/) (shell script in the `utilities` folder will install [juliaup](https://github.com/JuliaLang/juliaup) and initialize some packages for you as a simple alternative)
- [VSCode](https://code.visualstudio.com)


## Course Objective

The objective of this course is to familiarize you with computational methods for economics. In this course you should learn why we need computational methods for certain types of problems, the theory behind the methods, and most importantly, how to use them in practice. The first part of the course covers general basics of computing and doing computational research. The second part covers optimization and function approximation. The third part covers basic dynamic theory and a selection of methods for solving dynamic models. The fourth part covers basic spatial equilibrium models and how to solve them. 

I will be teaching the class in Julia. Julia is now widely used in computational economics because it's open source, it has many packages to employ the methods we will learn and practice, and it's fast and intuitive. **Please set up a GitHub (https://github.com) account before class starts.** Much of what we do can be easily ported to R, Python, MATLAB, and C.


## Integrity of credit

I expect every student in this course to abide by the Cornell University Code of Academic Integrity. I strongly encourage collaboration in this course, but each student is responsible for making sure that she or he follows the rules laid out in this syllabus, and with those stated in the Code of Academic Integrity. Any student found to have violated the stated policies on problem sets and papers will receive a zero for that assignment. Multiple violations in a semester may result in failure of the course. The Code of Academic Integrity is available for review here: https://cuinfo.cornell.edu/aic.cfm.

## Readings

Judd (1998) and Miranda and Fackler (2002) take a more detailed look at the fundamental numerical methods in economics. Nocedal and Wright (2006) is highly useful as a detailed reference for optimization. Judd (1998), Miranda and Fackler (2002), and Nocedal and Wright (2006) are available as eBooks in the library. Please look at
[Learning Julia](https://julialang.org/learning/) or go over the first few [QuantEcon Julia lectures](https://quantecon.org) for a brief introduction to coding in Julia. The remainder of the required readings will be from journal articles or excerpts from texts which will be accessible online and posted on GitHub a week before class.

Judd, Kenneth L. (1998) Numerical Methods in Economics, Cambridge, MA: MIT Press.

Miranda, Mario J. and Paul L. Fackler (2002) Applied Computational Economics and Finance, Cambridge, MA: MIT Press.

Nocedal, J. and S. J. Wright (2006) Numerical Optimization, New York: Springer, 2nd edition.

## Grading

- Class participation: 10%
- Presentation of a computational paper: 10%
- Final project proposal: 15%
- Final project paper/presentation: 25%
- Problem sets: 40%, 10% each

## Important dates

- Final project proposals due: March 17
- Final project presentations: Last week of class
- Final project due: May 19

## Assignments

### Problem sets
There will be four problem sets. You must submit your code on Canvas. You may work in a group of **two.** Each group should turn in one assignment with all members' names at the top of the file. Your grade will be a function of how well your answer the questions, and the clarity of your code (i.e. I should be able to tell what you're doing). I will help with conceptual issues on your problem sets but not minor coding issues. Part of the learning experience with problem sets is grappling with debugging code and learning how to use available resources (e.g. StackOverflow, ChatGPT).

- [Problem set 1:](https://raw.githack.com/AEM7130/class-repo/master/problem-sets/01-ps/01-ps.html) Due Feb 14 
- Problem set 2: Due TBD 
- Problem set 3: Due TBD 
- Problem set 4: Due TBD 

### Final project ([proposal instructions here](https://raw.githack.com/AEM7130/class-repo/master/final-project/project_proposal.html))

There is a final project for the course, due at the end of the semester. You may work in a group of two. You may choose one of two options below:

1. Begin a new computationally-driven research project. The project should:
  - Have an introduction that clearly states the economic question you are answering, frames your research in the context of the existing literature, and tells the reader what you are doing to advance economic knowledge.
  - Analytically develop the model, provide proofs for theoretical results if there are any.
  - Describe how you solve or estimate the model.
  - If possible, have preliminary results.
2. Expand an existing paper by bringing in advanced numerical techniques (i.e. not just adding MORE fixed effects). This can be your own paper (e.g. your current second year paper in progress), or an existing published paper where reproduction data and code are available online. AEA maintains a repository of data and code for all papers published in AEA journals [here](https://www.openicpsr.org/openicpsr/search/aea/studies). The paper should:
  - Briefly summarize the existing paper.
  - Describe the new techniques or data your are bringing to the table in detail.
  - Have preliminary results.
  - If using alternative techniques, compare outcomes or performance against the original methodology in the paper.

A 1-2 page proposal of the final project is due at about the halfway point of the course. During the final week of class, each student will present their completed work which should have a first-take at a numerical/empirical model and preliminary results.

### Computational paper presentations ([instructions here](https://raw.githack.com/AEM7130/class-repo/master/paper-presentation/paper-presentation.html))
Starting near the middle of the course, one student a class will present either a paper that either applies methods we have learned in a previous week, a paper that extends methods we have previously learned, or a package that is related to the methods we have learned. Presentations will be >15 minutes. Example applied papers are below for different sections of the course but you can choose to present another paper. All presentation topics must have my approval at least 1 week before the presentation date.

## Course Schedule

### Session 1: Intro to computing ([html](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/01-intro/01-intro.html)) ([pdf](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/01-intro/01-intro.pdf))

**Theory**: numbers, memory, linear algebra, calculus

Judd (1998, Chapters 2, 3 and 7)

Miranda and Fackler (2002, Chapters 1, 2, and 5)




### Session 2: Coding, reproducibility, and the shell ([html](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/02-coding/02-coding.html)) ([pdf](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/02-coding/02-coding.pdf))

**Applications**: shell scripts, julia speed, reproducibility, workflow

[Software Carpentry: The Unix Shell](https://swcarpentry.github.io/shell-novice/)

[AEA Reproducibility Guidance](https://aeadataeditor.github.io/aea-de-guidance/)

[Learning Julia](https://julialang.org/learning/)

[QuantEcon Lectures](https://quantecon.org/)




### Session 3: Version control ([html](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/03-git/03-git.html)) ([pdf](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/03-git/03-git.pdf))

**Applications**: git, github

[Software Carpentry: Version Control with Git](https://swcarpentry.github.io/git-novice/)

[SEERE Lab wiki](https://github.com/cornell-seere/lab-information/wiki)




### Session 4: Rootfinding and optimization ([html](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/04-optimization/04-optimization.html)) ([pdf](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/04-optimization/04-optimization.pdf))

**Theory**: iterative methods, newton methods, gaussian methods, global solvers

Judd (1998, Chapter 4 and 5)

Miranda and Fackler (2002, Chapters 3 and 4)

Nocedal and Wright (2006, Chapters 2-6)

**Applications**: transportation

Donaldson, Dave, and Richard Hornbeck. "Railroads and American economic growth: A “market access” approach." The Quarterly Journal of Economics 131, no. 2 (2016): 799-858.



### Session 5: Discrete time dynamic programming ([html](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/05-dynamic-programming/05-dynamic-programming.html)) ([pdf](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/05-dynamic-programming/05-dynamic-programming.pdf))

**Theory**: markov chains, principle of optimality

Adda, Jerome, Russell Cooper, and Russell W. Cooper. Dynamic economics: quantitative methods and applications. MIT press, 2003.

Ljungqvist, Lars, and Thomas J. Sargent. Recursive macroeconomic theory. MIT press, 2018.




### Session 6: Function approximation ([html](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/06-function-approximation/06-function-approximation.html)) ([pdf](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/06-function-approximation/06-function-approximation.pdf))

**Theory**: discretization, pseudospectral methods, finite element methods

Fernández-Villaverde, Jesús, Juan Francisco Rubio-Ramírez, and Frank Schorfheide. "Solution and estimation methods for DSGE models." In Handbook of macroeconomics, vol. 2, pp. 527-724. Elsevier, 2016.

**Application**: agriculture and climate change

Ortiz-Bobea, Ariel, Erwin Knippenberg, and Robert G. Chambers. "Growing climatic sensitivity of US agriculture linked to technological change and regional specialization." Science advances 4, no. 12 (2018): eaat4343.




### Session 7: Approximating value and policy functions for discrete time models ([html](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/07-dp-solution-methods/07-dp-solution-methods.html)) ([pdf](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/07-dp-solution-methods/07-dp-solution-methods.pdf))

**Theory**: value function iteration, policy iteration, time iteration

Aruoba, S. Borağan, Jesus Fernandez-Villaverde, and Juan F. Rubio-Ramirez. "Comparing solution methods for dynamic equilibrium economies." Journal of Economic dynamics and Control 30, no. 12 (2006): 2477-2508.

Cai, Yongyang, and Kenneth L. Judd. "Advances in numerical dynamic programming and new applications." In Handbook of computational economics, vol. 3, pp. 479-516. Elsevier, 2014.

Fernández-Villaverde, Jesús, Juan Francisco Rubio-Ramírez, and Frank Schorfheide. "Solution and estimation methods for DSGE models." In Handbook of macroeconomics, vol. 2, pp. 527-724. Elsevier, 2016.

**Applications**: climate change, bioeconomics

Cai, Yongyang, and Thomas S. Lontzek. "The social cost of carbon with economic and climate risks." Journal of Political Economy 127, no. 6 (2019): 2684-2734.


### Session 8: Continuous time optimal control ([html](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/08-optimal-control/08-optimal-control.html)) ([pdf](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/08-optimal-control/08-optimal-control.pdf))

**Theory**: maximum principle, hamiltonians, shooting, backwards shooting

Judd (1998, Chapter 10)

Caputo, Michael R. Foundations of dynamic economic analysis: optimal control theory and applications. Cambridge University Press, 2005.

**Applications**: oil extraction, climate policy

Anderson, Soren T., Ryan Kellogg, and Stephen W. Salant. "Hotelling under pressure." Journal of Political Economy 126, no. 3 (2018): 984-1026.

Lemoine, Derek, and Ivan Rudik. "Steering the climate system: using inertia to lower the cost of policy." American Economic Review 107, no. 10 (2017): 2947-57.


### Session 9: Advanced dynamic programming methods ([html](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/09-advanced-dp-methods/09-advanced-dp-methods.html)) ([pdf](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/09-advanced-dp-methods/09-advanced-dp-methods.pdf))

**Theory**: endogenous grid method, envelope conditions, modified policy iteration

Carroll, Christopher D. "The method of endogenous gridpoints for solving dynamic stochastic optimization problems." Economics letters 91, no. 3 (2006): 312-320.

Maliar, Lilia, and Serguei Maliar. "Envelope condition method versus endogenous grid method for solving dynamic programming problems." Economics Letters 120, no. 2 (2013): 262-266.

### Session 10: Solving spatial equilibrium models ([html](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/10-spatial-models/10-spatial-models.html)) ([pdf](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/10-spatial-models/10-spatial-models.pdf))

**Theory**: armington, eaton-kortum, exact hat algebra

Dekle, Robert, Jonathan Eaton, and Samuel Kortum. "Global rebalancing with gravity: Measuring the burden of adjustment." IMF Staff Papers 55, no. 3 (2008): 511-540.

Costinot, Arnaud, and Andrés Rodríguez-Clare. "Trade theory with numbers: Quantifying the consequences of globalization." In Handbook of international economics, vol. 4, pp. 197-261. Elsevier, 2014.

**Applications**: pollution regulation

Shapiro, Joseph S., and Reed Walker. "Why is pollution from US manufacturing declining? The roles of environmental regulation, productivity, and trade." American Economic Review 108, no. 12 (2018): 3814-54.


### Session 11: Solving dynamic spatial equilibrium models ([html](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/10-spatial-models/10-spatial-models.html)) ([pdf](https://raw.githack.com/AEM7130/class-repo/master/lecture-notes/10-spatial-models/10-spatial-models.pdf))

**Theory**: dynamic hat algebra

Caliendo, Lorenzo, Maximiliano Dvorkin, and Fernando Parro. "Trade and labor market dynamics: General equilibrium analysis of the china trade shock." Econometrica 87, no. 3 (2019): 741-835.

Kleinman, Benny, Ernest Liu, and Stephen J. Redding. "Dynamic spatial general equilibrium." Econometrica, (Forthcoming).

**Applications**: sea level rise

Balboni, Clare (2020) "In harm's way? infrastructure investments and the persistence of coastal cities."

### Session 12: Final project presentations
