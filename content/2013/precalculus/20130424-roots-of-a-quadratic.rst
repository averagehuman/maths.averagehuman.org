
Roots of a Quadratic Equation
=============================

:date: 2013-04-24 09:46
:author: averagehuman
:category: Precalculus
:latex:

The Quadratic Formula
---------------------

Consider the general quadratic equation:

.. math::

    ax^2 + bx + c = 0 \text{ (where } a, b, c \in \mathbb{R} \text { and } a \neq 0 \text{ )})

We want to find a formula for $x$ in terms of $a$, $b$, and $c$.

First rewrite as follows:

.. math::

    \begin{array}{rlr}
    \\
    x^2 + \frac{b}{a}x + \frac{c}{a} &= 0 \\
    x^2 + \frac{b}{a}x &= -\frac{c}{a} \\
    x^2 + \frac{b}{a}x + \left(\frac{b}{2a}\right)^2 &= -\frac{c}{a} + \left(\frac{b}{2a}\right)^2 \\
    \left(x + \frac{b}{2a}\right)^2 &= -\frac{c}{a} + \left(\frac{b}{2a}\right)^2
    \end{array}

Now we can solve for x:

.. math::

    \begin{array}{rlr}
    \\
    x + \frac{b}{2a} &= \pm \sqrt{-\frac{c}{a} + \left(\frac{b}{2a}\right)^2}\\
    x &= -\frac{b}{2a} \pm \sqrt{-\frac{c}{a} + \left(\frac{b}{2a}\right)^2}
    \end{array}

This can be further simplified by multiplying the right-hand side by $2a/2a$:

.. math::

    x = \frac{-b \pm \sqrt{-(c/a) \times (2a)^2 + (b/2a)^2 \times (2a)^2}}{2a}

giving the familiar formula:

.. container:: panel highlight

    .. math::

        x = \dfrac{-b \pm \sqrt{b^2 - 4ac}}{2a}

It follows that the two roots of a quadratic are:

+ real and unequal
+ real and equal
+ complex (imaginary)

according to whether the quantity $b^2 - 4ac$ is positive, zero, or negative.

Sum and product of roots
------------------------

Let \\(\\alpha\\) and \\(\\beta\\) be the roots of the equation. Then

.. math::

    \begin{array}
    \\
    \alpha &= \frac{-b + \sqrt{b^2 - 4ac}}{2a} \\
    \beta &= \frac{-b - \sqrt{b^2 - 4ac}}{2a}
    \end{array}

Adding:

.. math::

    \begin{array}
    \\
    \alpha + \beta &= \frac{-b + \sqrt{b^2 - 4ac}}{2a} + \frac{-b - \sqrt{b^2 - 4ac}}{2a} \\
    &= \frac{-b + \sqrt{b^2 - 4ac} -b - \sqrt{b^2 - 4ac}}{2a} \\
    &= \frac{-b}{a}
    \end{array}

Multiplying:

.. math::

    \begin{array}
    \\
    \alpha\beta &= \left(\frac{-b + \sqrt{b^2 - 4ac}}{2a} \right)\left(\frac{-b - \sqrt{b^2 - 4ac}}{2a} \right) \\
    &= \frac{b^2 + b\sqrt{b^2 - 4ac} - b\sqrt{b^2 - 4ac} - (b^2 - 4ac)}{4a^2} \\
    &= \frac{4ac}{4a^2} \\
    &= \frac{c}{a}
    \end{array}


