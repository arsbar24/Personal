This is a project I completed as part of [CPSC 540](https://www.cs.ubc.ca/~schmidtm/Courses/540-W17/) (a graduate level course in Machine Learning) working with Allison Tai. We were instructed to investigate some technique/application of machine learning that interested us and write a [NIPS style](https://nips.cc/Conferences/2017/PaperInformation/EvaluationCriteria) paper about it. The final result is in the [Project write up file](https://github.com/arsbar24/Personal/blob/master/Machine-Learning/Project-write-up.pdf). I have yet to include the code used for the learning processes; these will be uploaded at a later date.

In this project, we explore methods of machine learning based on [Optimal Transportation](https://en.wikipedia.org/wiki/Transportation_theory_(mathematics)). Optimal transportation is a problem in mathematics that involves calculating the most efficient way to transport items in one distribution to another based on some location based cost. 
In machine learning the distributions are usually interpreted to be the test and sample data and the distance function is some simple measure of similarity between samples (this is described in detail by Courty et al. [here](https://arxiv.org/pdf/1507.00504.pdf)).

In this project we try several methods of possible improvement on these methods, and apply them to the [MNIST dataset](http://yann.lecun.com/exdb/mnist/). Namely, we investigate

1. Using a concave transportation cost.

2. Interpreting the optimal transportation cost as a measure of similarity between image to generate test samples.

3. Using the optimal transportation plan to recognize rotated images.

4. Applying optimal transportation to the convolutions of images (via a CNN).

Experimentally, we conclude that (1) provides a modest but statistically significant improvement in almost all settings, while (2) is a major improvement that is easily implemented, (3) was found to be practical, but our experiments were unsuited to the MNIST dataset (whose samples have relatively uniform location/orientation), and (4) was too sensitive for practical amounts of data (we propose work-arounds involving ReLu levels to reduce dimensionality).
