# Multi Objective Optimisation
This repository is dedicated to tutorials to learn and practice using Pareto Fronts 
as a means for Multi-Objective Optimisation.

## PyData Global 2020
<img src="https://global.pydata.org/assets/images/logo.png" width="300">

Welcome and thanks for attending this tutorial session!    
If you have just listened to the intro video feel free to dive into notebook via the Colab buttons in the Outline section.  
Otherwise, you might want to go over the TL;DR and Motivation sections to have a better understanding of what to expect from this tutorial.

### Outline  
* Welcome and Intro (5 minute [video](http://bit.ly/moo-youtube-intro))
* Introduction to Pareto Fronts  (13 minutes in 2 videos: [1](http://bit.ly/moo-youtube-pareto1), [2](http://bit.ly/moo-youtube-pareto2))
* Hands On: Pareto Fronts (35 minutes in 3 videos: [1](https://bit.ly/moo-youtube-handson-pf1), [2](https://bit.ly/moo-youtube-handson-pf2), [3](https://bit.ly/moo-youtube-handson-pf3)) 
<a href="https://bit.ly/pareto-front-colab" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="First: Open In Colab"/></a>
* Decision and Objective Space (3 minute [video](https://bit.ly/moo-youtube-decision-space))
* Introduction to Pareto Optimisation with Genetic Algorithms (12 minutes in 2 videos: [1](https://bit.ly/moo-youtube-ga1), [2](https://bit.ly/moo-youtube-ga2))
* Hands On: Pareto Optimisation with Genetic Algorithms (45 minutes in 5 videos [1](https://bit.ly/moo-youtube-handson-ga1), [2](https://bit.ly/moo-youtube-handson-ga2), [3](https://bit.ly/moo-youtube-handson-ga3), [4](https://bit.ly/moo-youtube-handson-ga4), [5](https://bit.ly/moo-youtube-handson-ga5)) <a href="https://bit.ly/genetic-algorithm-colab" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="First: Open In Colab"/></a>
* Summary and Discussion (5 minute [video](https://bit.ly/moo-youtube-summary))

Video recording times of the hands-on sessions are shorter than the allocated time.

### Main Take Aways From Hands The On Sessions

The notebooks will help you learn to solve for multiple objective optimisation problems and visualise results.


* In `01_knapsack 2D_exhaustive.ipynb` you will optimise for the knapsack problem in an exhaustive solution space. Here you will learn:
    * The limitations of the commonly practiced Single Objective Optimisation.  
    * Pareto Fronts: identifying by eye Pareto optimal solutions within a distribution as well as pseudocode for selecting these *Non-Dominated* solutions.
    * Optimisation concepts *Decision Spaces* and *Objective Spaces*. These concepts are useful to determine the applicability of Pareto Optimisation.
* In `02_knapsack_2D_stochastic.ipynb` you optimise for the knapsack problem in an intractable search space. Here you will learn:
    * Stochasticity and Pareto front approximations 
    * Genetic Algorithm basics with an emphasis on Pareto fronts as the selection function.   
    * To track the learning progress of a Genetic Algorithm by means of the evolution of Pareto front approximations.
    * Improving population diversity by niching.

## TL;DR
Optimising for multiple objectives is a non-trivial task, especially when they are in conflict. For example how can one best overcome the classic trade-off between quality and cost of production, when the monetary value of quality is not defined?  In this hands-on Python tutorial you will learn about Pareto Fronts and use them to optimise for multiple objectives simultaneously.

This hands-on tutorial is geared towards anyone interested in improving their optimisation skills (e.g, analysts, scientists, engineers, economists), in which you will learn and implement

The only requirements are basic usage of `numpy` and `matplotlib`. The maths required is highschool level. 

Here you will find Jupyter notebooks with which you will apply lessons and tools learned to the simple [Knapsack problem](https://en.wikipedia.org/wiki/Knapsack_problem). 
You will program for filling a bag with packages with the objective of minimising the bag weight while maximising its content value. 

<img src="https://upload.wikimedia.org/wikipedia/commons/f/fd/Knapsack.svg" width="200">



## Motivation
Multi-Objective Optimisation, also known as Pareto Optimisation, is a method to optimise for multiple parameters simultaneously. When applicable, this method provides better results than the common practice of combining multiple parameters into a single parameter heuristic. The reason for this is quite simple. The single heuristic approach is like horse binders limiting the view of the solution space, whereas Pareto Optimisation enables a bird’s eye view

Real world applications span from supply chain management, manufacturing, aircraft design to land use planning. For example when developing therapeutics, Pareto optimisation may help a biologist maximise protein properties like effectiveness and manufacturability while simultaneously minimising toxicity.

This hands-on tutorial is geared towards anyone interested in improving their optimisation skills (e.g, analysts, scientists, engineers, economists), in which you will learn and implement:

*  The limitations of the common practice of combining multiple parameters into one heuristic.
*  *Pareto Fronts*: the notion in which there may be a set of trade-off solutions which are considered equally optimal.   
* Application of the Pareto Front method to Evolutionary Algorithms to find optimal solutions in an intractable search space.
* Applicability in the real world

We will use Python and work in a Jupyter notebook environment. 





## More Resources
For those interested in material before the tutorial, I kindly refer you to:   
* [DEAP](https://deap.readthedocs.io/en/master/) - a package for quick prototyping of evolutionary algorithms  
* [Pymoo](https://pymoo.org/) - a package with multi-objective optimization algorithms 
*  [PyData London talk](https://www.youtube.com/watch?v=_9x4cmQWZ6g) and [its slides](https://drive.google.com/file/d/1UMPGkeA_Tsc5PYWktpjquhIhOa9OD8Gb/view).  
*  For those who want extra curriculum I highly suggest any paper on the topic by [Eckart Zitzler](https://scholar.google.ch/citations?user=GW8tPekAAAAJ&hl=de). His Ph.D thesis is an excellent read.  
* Pareto Front example in an [Excel workbook](http://www.vertexvortex.com/r/excel/Pareto_Frontier.xlsx) (provided by [vertexvortex from Reddit](https://www.reddit.com/r/excel/comments/104fcb/pareto_frontier/)). 
