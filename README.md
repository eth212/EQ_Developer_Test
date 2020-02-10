# EQ_Developer_Test The code is in EQ works test.ipynb

Problem 4a BONUS

This model was created by analyzing the data, thinking about what each metric represents, ranking the metrics in
order of importance, choosing the best mathematical function to score the metric, factoring in best functions to 
distribute the final score.

The popularity of each region was decided according to the realization that the further people will travel to reach
a POI indicates how popular it is. Also considering the amount of people going to the POI (volume) and how distributed
the populations are (are people travelling from all over the radius to the POI or just within a population cluster).

This model would be greatly improved by adding in a metric to determine the spacial distribution within the radius
relative to the circled area. Like if density considered how far apart each node was within the space


Metrics 

volume : How many people come [rank 1] - Tanh - high reward for above average value but diminishes outliers
radius : how far people will come [rank 2] - Linear 
std deviation : decent indicator of distribution (how non-clustered the area is) [rank 3] - Linear
avg distance : how far the people coming away will commute (will generally be close) (far average means people will travel further) [rank 4] - arctanh - high precidence on outliers 
density : people per radius [rank 5] - Linear


I would have completed 4.b but I am very busy with school (midterms) and extra curriculars currently, and need to allocate my time elsewhere.

Side Note: I really enjoyed this challenge, I found the data interesting and there seemed to be lots of extractable information

I wrote my functions and methods to demonstrate understanding and clearify which solution belongs to which problem, If this was production code I would have used libraries to speed up most of the calculations used and I would not have seperate "for" loops on each different step. 
