Bayesian Statistical Methods
============================

This section introduces basic Bayesian statistical methods, including concepts like Bayes' theorem, prior distributions, likelihood, and posterior distributions.

Introduction
------------

Bayesian statistics is an approach to inference in which probabilities express a degree of belief in an event. It is based on Bayes' theorem, which provides a way to update the probability of a hypothesis given new evidence.

Bayes' Theorem
--------------

Bayes' theorem is the foundation of Bayesian inference. It is expressed mathematically as:

.. math::

   P(H | E) = \frac{P(E | H) \cdot P(H)}{P(E)}

where:

- :math:`P(H | E)` is the posterior probability, or the probability of the hypothesis :math:`H` given the evidence :math:`E`.
- :math:`P(E | H)` is the likelihood, or the probability of observing :math:`E` given that :math:`H` is true.
- :math:`P(H)` is the prior probability of the hypothesis.
- :math:`P(E)` is the marginal likelihood, or the probability of observing the evidence.

### Example Calculation

Consider a scenario where we want to estimate the probability that a person has a particular disease (hypothesis :math:`H`) given a positive test result (evidence :math:`E`). The prior probability :math:`P(H)` is the prevalence of the disease in the population. The likelihood :math:`P(E | H)` is the probability of testing positive given that the person has the disease.

Prior, Likelihood, and Posterior Distributions
----------------------------------------------

In Bayesian inference, we start with a **prior distribution** representing our initial beliefs about the parameters before observing any data. We then use the observed data to calculate the **likelihood**, and finally, combine the prior and the likelihood to obtain the **posterior distribution**.

.. note::

   The posterior distribution represents the updated belief after considering the new data.

+--------------------+-----------------------------------------+----------------------------------------------------------------+
| **Component**      | **Definition**                          | **Example in Disease Testing**                                 |
+====================+=========================================+================================================================+
| Prior              | Initial belief about a parameter        | Disease prevalence rate                                        |
+--------------------+-----------------------------------------+----------------------------------------------------------------+
| Likelihood         | Probability of data given the parameter | Probability of testing positive if the person has the disease  |
+--------------------+-----------------------------------------+----------------------------------------------------------------+
| Posterior          | Updated belief after observing data     | Probability of having the disease given a positive test result |
+--------------------+-----------------------------------------+----------------------------------------------------------------+

Graphical Representation of Bayesian Updating
---------------------------------------------

The following is a placeholder for a graph that illustrates the process of Bayesian updating, where the prior and likelihood combine to form the posterior distribution.

.. figure:: ./img/bayes-example.png
   :align: center
   :alt: Bayesian updating process

   This graph illustrates how a prior distribution is updated to a posterior distribution after observing data.

Example of Bayesian Inference in Practice
-----------------------------------------

Consider a medical test with the following parameters:

- **Disease prevalence** (prior): 1%
- **Sensitivity** (true positive rate): 99%
- **Specificity** (true negative rate): 95%

Using Bayes' theorem, we can calculate the probability that a person has the disease given a positive test result. Here’s how:

.. math::

   P(\text{Disease | Positive}) = \frac{P(\text{Positive | Disease}) \cdot P(\text{Disease})}{P(\text{Positive})}

where:

.. math::

   P(\text{Positive}) = P(\text{Positive | Disease}) \cdot P(\text{Disease}) + P(\text{Positive | No Disease}) \cdot P(\text{No Disease})

Summary of Bayesian Inference Process
-------------------------------------

+----------------------+--------------------------------------------------------+
| **Step**             | **Description**                                        |
+======================+========================================================+
| Define the prior     | Specify initial beliefs about the parameters           |
+----------------------+--------------------------------------------------------+
| Collect data         | Gather new evidence                                    |
+----------------------+--------------------------------------------------------+
| Calculate likelihood | Compute the probability of observing the data given    |
|                      | the parameters                                         |
+----------------------+--------------------------------------------------------+
| Update posterior     | Combine prior and likelihood to get the posterior      |
+----------------------+--------------------------------------------------------+

Conclusion
----------

Bayesian methods provide a powerful framework for updating beliefs in light of new evidence. This approach is widely used in fields such as medicine, finance, and machine learning, where probabilistic reasoning and continuous learning from data are essential.

Further Reading:

- "Bayesian Data Analysis" by Andrew Gelman, John B. Carlin, et al.
- "Doing Bayesian Data Analysis" by John K. Kruschke
