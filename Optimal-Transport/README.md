# Project for ![MATH 566](http://www.math.ubc.ca/~yhkim/yhkim-home/teaching/Math566-OT-2017/OT-2017.html) (Theory of Optimal Transportation)

The goal was to make some original conjectures (without proofs) related to optimal transportation and write them up in a short (~3 pages) coherent report. 

I explored a regularized version of the transportation problem, with motivation from Machine Learning (it is closely related to ![my machine learning project](https://github.com/arsbar24/Personal/tree/master/Machine-Learning) which provides more details about this problem). This also has applications to network analysis in Economics--for example optimizing transportation when factoring in congestion utility (see section 4 ![here](http://dedekind.mit.edu/~dws/boulder/IMA-transport-Lecture-Notes.pdf)).

## Summary of project

The first two conjectures explore the existence and structure of optimal measures and its relation to the convexity of the chosen regularizer.

Conjecture 3 shows transportation in an intricate network can be broken down into interpolation problems on simpler networks.

Conjecture 4 is a standard result connecting marginal utility to substitution preferences, and is a consequence of Lemma 5 which states a result concerning the structure of the optimal tranportation plan, analogous to ![c-cyclical monotonicity](https://arxiv.org/pdf/1601.05608.pdf) in the non-regularised version of the problem.

On the last page I show a Maximum a Posteriori argument for using a negentropy regularizer (reliant on Lemma 5), and propose some additional questions that I found interesting. 
