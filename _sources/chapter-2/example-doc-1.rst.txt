Fundamentals of Calculus
========================

Calculus is a branch of mathematics focused on limits, functions, derivatives, integrals, and infinite series. This document provides an overview of key concepts.

Introduction
------------

In this section, we will cover:

- The concept of limits
- Understanding derivatives
- An introduction to integrals

Limits
------

A **limit** is the value that a function approaches as the input approaches some value.

.. math::

   \lim_{x \to a} f(x) = L

Where:

- :math:`f(x)` is a function.
- :math:`a` is the value that :math:`x` approaches.
- :math:`L` is the limit value.

Derivatives
-----------

The **derivative** represents the rate at which a function is changing at any given point and is defined as:

.. math::

   f'(x) = \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}

Properties of Derivatives:

+------------------------+----------------------------------------------+
| **Property**           | **Description**                              |
+========================+==============================================+
| Linearity              | :math:`(af + bg)' = af' + bg'`               |
+------------------------+----------------------------------------------+
| Product Rule           | :math:`(fg)' = f'g + fg'`                    |
+------------------------+----------------------------------------------+
| Chain Rule             | :math:`(f \circ g)' = (f' \circ g) \cdot g'` |
+------------------------+----------------------------------------------+

Integrals
---------

An **integral** assigns numbers to functions to describe displacement, area, volume, and other concepts.

Definite Integral:

.. math::

   \int_{a}^{b} f(x) \, dx

Where:

- :math:`a` and :math:`b` are the limits of integration.
- :math:`f(x)` is the integrand.
- :math:`dx` indicates integration with respect to :math:`x`.

Conclusion
----------

Calculus provides tools for modeling and solving problems involving change and motion, which are essential in physics, engineering, and economics.

Further Reading:

- "Calculus Made Easy" by Silvanus P. Thompson
- "A Brief History of Calculus" by Carl B. Boyer
