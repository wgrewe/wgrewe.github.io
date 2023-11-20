# Portfolio

Welcome to Weston Grewe's portfolio of projects. These projects range from applied data science (such as analyzing bike lanes in Denver) to pure mathematics. Please check out any of the projects below.

## About Me
Hi, I'm Weston! I am a Ph.D. candidate studying Operations Research at the University of Colorado Denver with an expected graduation date of May 2024.

For the last three years, I have been funded through a grant my advisor holds. Primarily, I research linear programming and combinatorial optimization. In particular, I am interested in polyhedral geometry, especially combinatorial diameters and circuit diameters. Combinatorial diameters provide lower bounds on the worst-case performance of the Simplex Method. Circuits generalize edges of a polyhedron, circuit augmentation schemes generalize the Simplex method. In a circuit augmentation scheme, an algorithm follows circuit directions. This is a trade off: there are more directions to choose from, so a run of the algorithm may need fewer iterations, but each direction is harder to compute. I study circuit diameters, which give a lower bound on the number of iterations a run of a circuit augmentation scheme may need.

Prior to my program at CU Denver, I completed a B.S. and M.S. in pure mathematics at Cal Poly, San Luis Obispo. I wrote a senior project where I studied functional analysis and the invariant subspace problem for compact operators. For my master's thesis I homogenized a cardiac tissue model to analyze large scale behavior of the tissue.

Aside from research, I have worked as a data science intern at Transamerica (Summer 2022/2023). This was a fascinating experience that introduced me to working with some very large datasets and various data science topics such as entity resolution, encoders/decoders, transfer learning and positive-unlabeled learning.

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

During this internship I worked on several projects spanning many facets of data science. 

For my first internship I worked on three projects. The first project was in network optimization. The COO of Transamerica wanted to develop a program to connect employees in operations to one another to boost networking and the sharing of ideas. The goal was to pair employees that are on different hierarchy levels and are separated in the company, i.e. pairing employees who do not have the same manager or whose manager's have the same manager. To accomplish this, we transformed the data into a graph and solved a maximum cardinality maximum weight matching problem on the graph.

The second project concerned finding complaints in call data. This is one of the largest projects the team is working on. The company recieves thousands of phone calls a day, and the call center representative can label a few topics pertaining to the call. The company would like to know which calls are complaints and what the complaints are about. We had a very small subset of the calls that we knew were complaints, therefore, supervised learning was a possibility, at least for prototyping. We investigated several methods such as positive-unlabeled learning and zero-shot learning. We also performed some analysis of the text to determine if the word distributions are meaningfully different.

The third project involved cleaning our Illustration database. Transamerica, as a life insurance company, generates an illustration for a potential client which contains specific proposed details for a policy, like an estimate for a service. Each illustration is stored in a database. Before this project, the database had no process for removing outdated illustrations. An illustration is outdated if a sufficient amount of time has passed or the customer bought the policy. The first case is easy, we set up a time-based filter. The seond is more challenging. We needed to match illustrations to policies. Illustrations are semi-structured text data. Agents are given a form to type in data, although, they are not mandated to use this form. Policies, thankfully, are stored as tabular data and have clear formatting guidelines. I applied entity resolution, with some probabilistic methods and some rules-based mathods, to match illustrations to policies. In the end, I decreased the size of the illustration data base by 60%.

In the following summer, I continued with the complaints project. This round, I worked with HuggingFace's pipelines to perform transfer learning on the data. I also explored other tokenization methods, such as TF-IDF and Doc2Vec. Further, I used a lightweight transformer, VAMPIRE, to compare results. Much of this work was also focused on the ML engineering side of data science: writing production-ready code. Further, this project also gave me experience with SQL. There is interest in knowing who the callers who made the complaints are. This involves joining data across several tables to find the correct identifier. 

My final project was a graphical approach to territory allocation. Each office is assigned a territory and there is a want for the sum-total of sales across offices to be balanced over each territory and that territories are compact, i.e., convex bodies with small perimeter to area ratio. This project allowed me to apply my research of circuit augmentation to an applied problem. Circuits provide a minimal change while still maintaining feasibility. By choosing a direction that points towards some optimal assignment, each reassignment changes the territory of just a few offices, and marches towards the optimal.

## Complexity of Constructing Short Circuit Walks

Many graph reconfiguration problems can be interpreted as circuit problems, especially matching, coloring, and clustering. Circuits give a practical answer for applied problems because each step often has a real world interpretation. Because of this applicability, there is some need for circuit walks with few steps (not too many changes are made) or circuit walks with a small geometric length (changes made are not too sweeping). We show that both finding circuit walk with the fewest steps and find the circuit walk with minimal length are NP-complete problems. However, we show for network-flow and TU polytopes these problems are easy. In the network-flow case, this reduces to cycle-finding in a graph. 

This work is currently in progress and will be uploaded to the ArXiv in the near future.

## 2-Sums of Polyhedra

This is a continuation of my work on combinatorial diameters of polyhedra. The 2-sum operation is fundamental in the construction of totally unimodular polyhedra, the easiest polyhedra for integer programming. The 2-sum can be interpreted as the linking of two systems in a joint model with a single constraint. Thus, a deep understanding of how the 2-sum affects the geometry of the polyhedron allows for the problem to be broken into two (hopefully easier) subproblems. We show that the diameter of the 2-sum polyhedra is at most quadratic in the diameters of its parts. In a sense, the linking of two simple systems through the 2-sum does not create a highly complex system.

Our work is currently submitted for publication. For much more detail and a more rigorous explanation, please see our article on the [ArXiv](https://arxiv.org/abs/2311.02047).

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



## Master's Thesis: Homogenization of a Cardiac Tissue Model



## Project Euler

I spent a whole summmer working on [Project Euler](https://projecteuler.net/) problems as a tool to hone my programming skills. Project Euler provides a nice blend of pure math questions with algorithms. Most of the questions cannot be answered by a brute force search, they require clever combinatorial techniques. Solutions to most of the first 100 can be found [here.](https://github.com/wgrewe/Project-Euler) While I have solved several of those past 100, Project Euler does not allow those solutions to be posted on the internet.


## Senior Project: Invariant Subspace Problem

In the good old days when I was a pure math undergrad, I studied functional analysis for my senior project. I studied the first 5 chapters of [MacCleur's book](https://link.springer.com/book/10.1007/978-0-387-85529-5#toc) and worked on a proof of the invariant subspace problem for compact operators. An invariant subspace is a generalization of an eigenvector and has far-reaching implications throughout functional analysis and the theory of linear operators. Compact operators are some of the nicest operators on an infinite dimensional vector space while still maintaining interesting properties. Particularly, many results that hold for square matrices hold for compact operators, thus, intuition about how these operators work transfer nicely. This is often not the case in infinite dimensional space. My work for this project can be found [here.](https://digitalcommons.calpoly.edu/mathsp/7/) 
