# Portfolio

Welcome to Weston Grewe's portfolio of projects. These projects range from very applied data science (such as analyzing bike lanes in Denver) to pure mathematics. Please check out any of the projects below.

## About Me
Hi, I'm Weston! I am a PhD student in Operations Research at the University of Colorado Denver with an expected graduation data of Dec 2023.

My primary research areas are linear programming and combinatorial optimization. In particular, I am very interested in diameters of polyhedra and circuit augmentation algorithms. Prior to my program at CU Denver, I completed a BS and MS in pure mathematics at Cal Poly San Luis Obispo. I wrote a senior project where I studied functional analysis and the invariant subspace problem for compact operators. For my master's thesis I homogenized a cardiac tissue model to analyze large scale behavior of the tissue.

Aside from research, I have worked as a data science intern at Transamerica (Summer 2022). This was a fascinating experience that introduced me to working with some very large datasets and various data science topics such as entity resolution, encoders/decoders, and positive-unlabeled learning.

Following graduation I hope to break into the data science industry.  

## Here are some quick links to my repositories
### Check back soon for actual links
- Internship at TA
- Biking in Denver (done)
- Paper on ArXiv (done)
- Spatial Statistics
- Circuit Walks
- Integer Programming
- Linear Programming
- Spam Filter
- Project Euler
- Senior Project
- Master's Thesis

## Data Science Internship at Transamerica

During this internship I worked on 3 projects. The first project was a network optimization problem. The COO wanted to develop a program to connect employees in operations to one another to boost networking and the sharing of ideas. The goal was to pair employees that are on different hierarchy levels and are separated in the company, i.e. pairing employees who do not have the same manager or whose manager's have the same manager. To accomplish this, we transformed the data into a graph and solved a maximum cardinality maximum weight matching problem on the graph.



## Safe Biking in Denver

In the spring of 2022 I participated in the Data to Policy Symposium hosted by the Auraria Library. My peer [Angela Morrison](http://math.ucdenver.edu/~sborgwardt/wiki/index.php/Angela_Morrison) and I analyzed the feasibility of commuting in Denver. We used a generic shortest path algorithm and a cost-constrained shortest path algorithm to understand the burden that riders face when commuting in the city. We are pleased to report that our project won Best in Data. For a full description of our work please visit our [project page.](http://math.ucdenver.edu/~sborgwardt/wiki/index.php/A_Wheelie_Good_Time:_Safe_Biking_in_Denver) For data cleaning and analysis please see our [GitHub Repository.](https://github.com/DillWithIt77/D2P_Spring_2022) 

## Diameters of Connections of Polyhedra

As part of my PhD thesis, I have been researching diameters of polyhedra. Polyhedral diameters provide a lower bound on the number of pivots the simplex method would take, independent of pivot rule. We proved diameter bounds for polyhedra whose constraint matrix is either a parallel connection or series connection of matrices. The parallel connection and series connection characterize behavior for an optimization problem that has a constraint or variable linking two independent processes. Our work is currently submitted for publication, a preprint is available on [Arxiv.](https://arxiv.org/abs/2203.09587)

## Childhood Obesity in the City of Denver

In the fall of 2021 I submitted two projects to the data to policy symposium. This project is associated with CU Denver's Spatial Data Analysis course. Using data from Denver's Open Data Catalog, I analyzed the distribution of childhood obesity throughout the city to discover if there were any clusters. After performing 6 seperate statistical tests, I discovered there was evidence of clustering. In particular, central north Denver, southwest Denver, and Montbello all exhibited evidence of clustering of childhood obesity cases. My work can be found in [this github repository.](https://github.com/wgrewe/Childhood-Obesity) A slide deck of the results can be found [here.](https://digital.auraria.edu/work/ns/ae3a1cef-3823-44ab-8e54-8a198e58b9a6) 


## Which Neighborhoods in Denver are Experiencing Gentrification?

It is no secret that Denver has experienced incredible gentrification over the last decade. As one of the fastest growing cities since 2010, housing supply has been ravaged. I will always credit Denver for allowing homebuilding to be a comparatively easy process. Regardless, when any city is growing as fast Denver has, keeping up with housing demand will be near impossible. 

This project arose as a unique (although, ultimately unsuccessful) way to understand gentrification. In particular, it may be useful as a prediction engine for determining where gentrification will occur next. A predication engine for gentrification is vital, often neighborhoods impacted by gentrification are unnoticed until it is too late. Our project considers 3 different time points in Denver and clusters (using k-means) neighborhoods into 3 categories: marginalized, neutral, and privileged. To do so we consider income, education, and..

Now, we dive into the mathematics. Once we clustered, we considered sign-compatible circuit walks between clustered. This circuits walks provide a ``transition'' between clusters. They yield a sequence of clusters that begin at one cluster and each intermediary cluster differs by just interchanging the labels of at most 2 neighborhoods. Hence, we have recovered how one cluster turned into another several years down the road.

## An Optimal Decision Tree Model for College Enrollment

For CU Denver's Data to Policy Symposium in spring of 2021, we investigated which factors led to a high college enrollment. We used data from Massachusetts Public Schools and used an optimal decision tree model. The decision tree model was described in [this article](https://optimization-online.org/2018/01/6404/). The decision tree can be computed by solving an integer linear program. We programmed this model in AMPL and designed it to read data from an Excel table. 

## A Mathematical Approach to Prevent Gerrymandering


## A Basic Email Spam Filter 


## Master's Thesis: Homogenization of a Cardiac Tissue Model



## Project Euler

I spent a whole summmer working on [Project Euler](https://projecteuler.net/) problems as a tool to hone my programming skills. Project Euler provides a nice blend of pure math questions with algorithms. Most of the questions cannot be answered by a brute force search, they require clever combinatorial techniques. Solutions to most of the first 100 can be found [here.](https://github.com/wgrewe/Project-Euler) While I have solved several of those past 100, Project Euler does not allow those solutions to be posted on the internet.


## Senior Project: Invariant Subspace Problem

In the good old days when I was a pure math undergrad, I studied functional analysis for my senior project. I studied the first 5 chapters of [MacCleur's book](https://link.springer.com/book/10.1007/978-0-387-85529-5#toc) and worked on a proof of the invariant subspace problem for compact operators. An invariant subspace is a generalization of an eigenvector and has far-reaching implications throughout functional analysis and the theory of linear operators. Compact operators are some of the nicest operators on an infinite dimensional vector space while still maintaining interesting properties. Particularly, many results that hold for square matrices hold for compact operators, thus, intuition about how these operators work transfer nicely. This is often not the case in infinite dimensional space. My work for this project can be found [here.](https://digitalcommons.calpoly.edu/mathsp/7/) 
