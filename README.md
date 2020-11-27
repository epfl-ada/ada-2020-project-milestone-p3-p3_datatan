# ada-2020-project-milestone-p3-p3_datatan
ada-2020-project-milestone-p3-p3_datatan created by GitHub Classroom


Title: Trust and distrust propagation in signed network 

Abstract: 
We want to focus our attention on the “signed” aspect of the networks. To do so we decided to treat the three datasets of the paper as “webs of trust”. The basic concept is to allow each node of the network to vote for his neighbours (+1 Trust, -1 Distrust) and observe which are the nodes with the highest score of trust/distrust (and the characteristics of the regions close to those nodes). Then we want to go a step forward and try to propagate trust between nodes that are not connected (using multiple models), after the propagation we will be able to compare the high trust/distrust regions between different propagation models and within the no-propagation case.  
The story that we want to tell is about uncovering the real
trust/distrust distribution in a network and show that consensus is more subtle
than the simple count of positive edges around a node.  

Research Questions:
Correlation between nodes with high trustworthiness and zones with high “all positives” triads / % “+” edges.
The supposition that “the friend of my friend is my friend” is confirmed by trust propagation models ?
How do different propagation models compare to each other when we investigate the distribution of trust/distrust ? 
Does the “reputation hypothesis” hold on the basis of trust (example: A trust B, B trusts C, if C has a trust score greater than A, should A trust C)? 
Proposed dataset: Epinions, Slashdot and Wikipedia, from the paper of the signed network project:
https://cs.stanford.edu/people/jure/pubs/triads-chi10.pdf 

Methods:
Load the datasets and ensure that each edge is signed +1 or -1.
Assign a trust score score to each node of the network based on the sign of the edges in his neighbourhood.
Build the propagation models (functions). Each propagation model increases the trust value of the node:
Direct propagation: a trust b, b trust c, so a trust c 
Co-citation: a trust b,  a trust c, d trust c, so d trus b   
Transpose trust : a trust b, c trust b, so c trust a 
Trust coupling: a and b trust c,  d trust a, so d trust b 
Display the trust scores for each node and for each propagation model.
Perform edge/triad count of the new graphs (with the new edges added by the propagation).
Compute statistics between the different counts and drown conclusions on viability of trustiness propagation as an indicator of trust distribution in signed networks.     

Timeline:
Week 1:  Load the data and make sure that the dataset is viable as a network. Build a system that is able to count the trust level of each node. Define the functions that will propagate the trust.     
Week 2: Code and optimize the functions that propagate the trust, make sure that everything works as expected. Visualize the results and perform the statistics.
Week 3: Write the conclusions and do the individual part of the project.

Organization:
Alexandra: 
Week 1: code the models for the trust propagation. 
Week 2: code the models for the trust propagation.
Week 3: Discuss the conclusions.
Robert: 
Week 1: Count of the trust of each node.
Week 2: Perform statistics.
Week 3: Discuss the conclusions.
Lorenzo: 
Week 1: Load the data (data wrangling).
Week 2: Visualize the results graphically. 
Week 3: Discuss the conclusions.
  
    









